# 🚀 AI-Powered E-commerce Image Generation Workflow

![n8n](https://img.shields.io/badge/n8n-Workflow_Automation-ff6d5a?style=for-the-badge&logo=n8n&logoColor=white)
![Google Vertex AI](https://img.shields.io/badge/Vertex_AI-Gemini_Models-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![AI](https://img.shields.io/badge/AI-Generative_AI-black?style=for-the-badge)
![Automation](https://img.shields.io/badge/Automation-End_to_End-blueviolet?style=for-the-badge)

Transform a simple clothing photo into studio-quality product images and lifestyle shots using AI-driven automation.

This project demonstrates an end-to-end workflow built with **n8n**, integrating **Google Vertex AI (Gemini models)** and image generation APIs to automate fashion product photography.

---

## 📌 Overview

E-commerce businesses often rely on expensive photoshoots and manual editing.  
This workflow replaces that with an automated, scalable pipeline:

👉 Upload a basic clothing image → get multiple high-quality product images ready for use.

---

## 🎯 Features

- 📸 Convert low-quality clothing images into professional visuals  
- 🤖 AI-generated photorealistic models wearing the product  
- 🎬 Automatic generation of multiple scene variations  
- 🧠 Meta-prompting for dynamic prompt creation  
- 🗂️ Auto folder creation with structured naming (Google Drive)  
- 🔄 Fully automated workflow using n8n  

---

## ⚙️ Tech Stack

| Component | Purpose |
|----------|--------|
| n8n | Workflow orchestration |
| Google Vertex AI (Gemini) | AI reasoning + prompt generation |
| Gemini Flash Image Model | Image generation |
| Google Drive API | Storage & organization |

---

## 🧠 Model Roles in the Workflow

This system uses a dual-model architecture:

| Model | Role | Purpose |
|------|------|--------|
| gemini-2.5-pro | 🧠 Brain | Prompt generation, analysis, meta-prompting |
| gemini-2.5-flash-image | 🎨 Artist | Image generation |

👉 Conceptually: AI (thinking) → AI (creating)

- One model decides what to create  
- Another model actually creates it  

This separation improves both quality and flexibility.

---

## 🧠 Workflow Architecture
<img width="185" height="172" alt="image" src="https://github.com/user-attachments/assets/2e7e73ab-662d-4bf3-ac31-9039f855f896" />


---

## 🔄 How It Works

### 1. Input

A simple image of a clothing item (mobile photo works).

---

### 2. Model Generation

AI generates a realistic human model wearing the exact garment.

- Maintains garment accuracy (color, texture, fit)  
- Avoids redesign or hallucination  

---

### 3. Meta-Prompting (Core Logic)

Instead of writing static prompts, this workflow uses meta-prompting.

---

### 💡 What is Meta-Prompting?

Meta-prompting is a technique where:

👉 AI is instructed to generate prompts for another AI

Instead of: Human → writes prompt → Image generated

It becomes:

<img width="175" height="66" alt="image" src="https://github.com/user-attachments/assets/16ab7137-cce1-4c9b-a180-482cda4591d6" />


---

### 🧠 Why Meta-Prompting is Important

Meta-prompting solves key real-world problems:

#### 🔄 Handles Variety
- Works for jeans, shirts, jackets, etc.  
- Adapts automatically based on input image  

#### 🎯 Adds Domain Expertise
- AI uses photography concepts (lighting, angles, composition)  
- Produces results closer to professional shoots  

#### 📈 Scales Content Creation
- Generates multiple scene ideas instantly  
- No manual brainstorming needed  

---

### 4. Image Generation

Two categories of outputs:

#### 🏢 Studio Shots
- Front view  
- Side/angle view  
- Back view  
- Detail close-up  

#### 🌆 Lifestyle Shots
- Context-aware environments  
- Real-world usage scenarios  
- Marketing-ready visuals  

---

### 5. Storage & Organization

- Creates a unique folder per run  
- Uses sequential naming  
- Stores all generated images in Google Drive  

Example:
<img width="83" height="60" alt="image" src="https://github.com/user-attachments/assets/72727b4c-feca-44c6-87e4-cc4582f35f34" />


---

## 🧪 Example Use Cases

- E-commerce product listings  
- Fashion catalogs  
- Marketplace sellers (Amazon, Shopify, etc.)  
- Automated content pipelines  

---

## 📂 Project Structure (n8n Flow)

1. Upload / Input Node  
2. Image Processing (Base64 conversion)  
3. AI Model Generation  
4. Meta Prompt Generation  
5. Image Generation API Call  
6. Convert Base64 → Binary  
7. Create Folder (Google Drive)  
8. Upload Images  

---

## ⚠️ Challenges & Learnings

- Handling binary vs JSON data flow in n8n  
- Managing rate limits (429 errors) in AI APIs  
- Ensuring exact garment consistency in generated images  
- Designing robust and reusable prompt pipelines  

---

## 🚀 Future Improvements

- Video generation from output images  

---

## 🎬 Demo

*(Add demo video / GIF here)*

---

## 🤝 Contributing

This project is part of ongoing experimentation and learning.  
Suggestions, improvements, and ideas are welcome.

---

## 📜 License

MIT License (or update as needed)

---

## 🙌 Acknowledgement

Special thanks to @LucasWalterAI for sharing insights and workflows that inspired this project.  
This implementation was built and customized as part of my own learning and development.
- AI workflows  
- Automation systems  
- E-commerce optimization  




