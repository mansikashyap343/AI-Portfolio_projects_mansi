**Multimodal Emotional & Personality Analysis from Screenshots**

This project is a multimodal AI system that analyzes screenshots containing text (example: chat conversations) and produces emotional, sentiment, and personality insights, followed by an AI-generated counselor style summary. 

**Project Overview**

The system combines:

Computer Vision (OCR)

NLP with Transformer models

Classical Machine Learning

Rule-based AI interpretation

It simulates how an AI counselor might interpret emotional and personality signals from everyday text.

**Features**

OCR text extraction from screenshots

Sentiment analysis using RoBERTa

Emotion classification (28 emotion classes)

Big Five personality prediction

AI-generated counselor summary

Beginner-friendly Google Colab workflow

**How It Works**
**OCR Extraction**

Text is extracted from uploaded screenshots using EasyOCR.

**Sentiment & Emotion Analysis**

Transformer models used:

cardiffnlp/twitter-roberta-base-sentiment

j-hartmann/emotion-english-distilroberta-base

**Personality Prediction**

A custom classical ML pipeline:

TF-IDF Vectorizer

Logistic Regression

Predicts dominant Big Five traits

**AI Counselor Summary**

A rule-based system synthesizes:

Emotional tone

Personality indicators

Supportive psychological insight

**Example Output**

Sentiment: Positive
Top Emotions: Joy, Relief, Approval
Dominant Trait: Agreeableness

**AI Counselor Insight**

The message reflects warmth and cooperation, indicating emotional stability and positive social engagement.

**Tech Stack**
Computer Vision

EasyOCR

Pillow

NLP

Hugging Face Transformers

RoBERTa

Machine Learning

TF-IDF

Logistic Regression

scikit-learn

Runtime

Google Colab

**Files**

ocr_nlp_analyzer.ipynb — Main notebook

README.md — Documentation
