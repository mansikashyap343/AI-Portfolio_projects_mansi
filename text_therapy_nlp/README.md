OCR + NLP Emotional & Personality Analyzer

A multimodal AI tool that reads screenshots, extracts text, and performs personality, sentiment, and emotion analysis, followed by a final AI-generated counselor-style summary.

1. Project Overview

This project demonstrates a complete multimodal AI pipeline:

User uploads a screenshot (chat/text message).

OCR extracts text using EasyOCR.

Transformer models perform:

Sentiment classification

Emotion classification (28-class)

A local classical ML model predicts Big Five personality traits using TF-IDF + Logistic Regression.

A final AI counselor summary interprets:

Emotional tone

Personality markers

Supportive insight

This project showcases integration of computer vision + NLP + classical ML + prompt-based interpretation.

2. Features

Extract text from screenshots using OCR

Analyze sentiment using a RoBERTa transformer model

Detect top emotions with a transformer-based emotion classifier

Predict Big Five personality traits using a custom ML classifier

Generate an AI counselor report combining all signals

Simple, beginner-friendly workflow in Google Colab

3. Tech Stack
A. Computer Vision

EasyOCR

Pillow

B. NLP Models

Hugging Face Transformers

RoBERTa sentiment model

DistilRoBERTa emotion classifier

C. Machine Learning

TF-IDF Vectorizer

Logistic Regression

NumPy / scikit-learn

D. Runtime

Google Colab (file upload widget)

4. How It Works
4.1 Upload a Screenshot
from google.colab import files
uploaded = files.upload()
image_path = list(uploaded.keys())[0]

4.2 OCR Extraction
ocr_reader = easyocr.Reader(['en'])
results = ocr_reader.readtext(image_path, detail=0)
extracted_text = " ".join(results)

4.3 Sentiment & Emotion Analysis

Models used:

cardiffnlp/twitter-roberta-base-sentiment

j-hartmann/emotion-english-distilroberta-base

sentiment = run_nlp(extracted_text, sentiment_model, sentiment_tokenizer, sentiment_labels)
top_emotions = run_nlp(extracted_text, emotion_model, emotion_tokenizer, emotion_labels)

4.4 Personality Prediction (Custom ML Model)

A small in-notebook dataset is used for proof-of-concept:

vectorizer = TfidfVectorizer()
personality_models = {...}
personality = predict_personality(extracted_text)

4.5 AI Counselor Summary

A rule-based summary combines:

Sentiment

Top emotion

Dominant personality trait

ai_summary = ai_counselor_summary(extracted_text, personality, sentiment, top_emotions)

5. Example Output

Extracted Text:
“Hey, what time is our reservation tonight?”
"Hi! I got us a table for 7p.m."
"Sounds good. See you soon"


Sentiment:
positive

Top Emotions:
joy, relief, approval

Personality Pattern:
Agreeableness dominant

AI Counselor Summary (Sample):

Emotional Tone: The message expresses joy with a positive sentiment.

Personality Indicators: The strongest trait is Agreeableness. The language reflects cooperation and warmth.

Support Insight: The tone is relaxed and reassuring, indicating emotional stability.
