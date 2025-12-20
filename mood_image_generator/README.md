**Mood-Based Image Generation with Stable Diffusion**

This project generated AI images based on a user's emptional state while using a prompt template. By entering a single mood word (example: happy, calm, melancholic, sad etc), the system produces an AI-generated artwork that visually represents the very emotion. 

**Project Idea**

Many people experience emotions intensely but struggle to visualize them!!
This project bridges that gap by translating abstract emotional states into concrete visual representations using generative AI.

A fixed prompt template ensures:

stylistic consistency

high image quality

controlled aesthetic output

**Features**

Mood-to-image generation using prompt engineering

Simple text-based user input

Compatible with Stable Diffusion–based models

Automatically displays and saves generated images

Easy customization of artistic style and aesthetics

**How It Works**

User inputs a mood (e.g., "happy", "calm", "angry")

The mood is injected into a predefined prompt template

Stable Diffusion generates an image reflecting the emotion

The output image is displayed and saved locally

**Prompt Template Used**
"A detailed, cinematic, high-quality digital artwork that represents the mood: {mood}. 
Vibrant colors, artistic composition, smooth textures, and dramatic lighting."


You can easily modify the template to generate:

anime-style art

watercolor paintings

oil paintings

photorealistic images

**How to Run**

Install required dependencies:

diffusers

torch

transformers

pillow

Open the notebook:

ImageryTherapy_GITHUB_READY.ipynb


Run all cells

Enter a mood when prompted

View and save the generated image

**Files**

ImageryTherapy_GITHUB_READY.ipynb — Main notebook

README.md — Project documentation
