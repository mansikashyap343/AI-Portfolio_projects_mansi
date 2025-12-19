# Mood-Based Image Generation

This project generates AI images based on a user's mood using a fixed prompt template.  
By entering a mood (e.g., *happy*, *calm*, *melancholic*, *romantic*), the notebook feeds the mood into a predefined prompt structure and produces an image that visually represents the emotion.

---

## 📌 Project Idea

Many people feel emotions strongly but struggle to visualize them.  
This project translates a **single mood word** into an **AI-generated artwork** using a consistent prompt template that ensures clarity, quality, and style control.

---

## ✨ Features

- Mood-to-image generation using a fixed prompt structure  
- Clean and simple user input  
- Compatible with models like **Stable Diffusion / DALL·E**  
- Saves output images automatically  
- Easy to modify the default aesthetic or style  

---

## 🧠 How It Works

1. User enters a mood → `"happy"`, `"calm"`, `"angry"`, etc.  
2. Mood is inserted into a **template prompt**, such as:  
   *"A highly detailed artistic illustration representing the mood: {mood}. Soft lighting, high resolution, cinematic atmosphere."*
3. The image generation model produces an artwork based on the mood.
4. The result is displayed and saved.

---
# Mood-Based Image Generation

This project generates AI images based on a user's mood using a fixed prompt template.  
By entering a mood (e.g., *happy*, *calm*, *melancholic*, *romantic*), the notebook feeds the mood into a predefined prompt structure and produces an image that visually represents the emotion.

---

## 📌 Project Idea

Many people feel emotions strongly but struggle to visualize them.  
This project translates a **single mood word** into an **AI-generated artwork** using a consistent prompt template that ensures clarity, quality, and style control.

---

## ✨ Features

- Mood-to-image generation using a fixed prompt structure  
- Clean and simple user input  
- Compatible with models like **Stable Diffusion / DALL·E**  
- Saves output images automatically  
- Easy to modify the default aesthetic or style  

---

## 🧠 How It Works

1. User enters a mood → `"happy"`, `"calm"`, `"angry"`, etc.  
2. Mood is inserted into a **template prompt**, such as:  
   *"A highly detailed artistic illustration representing the mood: {mood}. Soft lighting, high resolution, cinematic atmosphere."*
3. The image generation model produces an artwork based on the mood.
4. The result is displayed and saved.

---

## 🧩 Prompt Template Used

"A detailed, cinematic, high-quality digital artwork that represents the mood: {mood}.
Vibrant colors, artistic composition, smooth textures, and dramatic lighting."

yaml
Copy code

You can change the style (anime, watercolor, oil painting, photorealistic) by editing the template.

---

## 🚀 How to Run the Notebook

1. Install required libraries:
   - diffusers / openai / stable diffusion (based on your model)
   - torch
   - pillow
   - matplotlib

2. Open `mood_image_generator.ipynb`

3. Run all cells:
   - When prompted, enter a mood  
   - The notebook generates and displays an image  
   - The image is saved inside the notebook directory

---

## 📁 Files in This Folder

- `mood_image_generator.ipynb` — main notebook  
- `README.md` — documentation  


