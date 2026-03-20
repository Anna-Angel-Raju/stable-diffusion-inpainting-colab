# 🎨 Image Inpainting using Stable Diffusion

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-DeepLearning-red)
![HuggingFace](https://img.shields.io/badge/HuggingFace-Diffusers-yellow)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

---

## 🚀 Run in Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/132Oeq4rRKaQ6GhblgENZVEoUTP2EXzc2)

---

## 🧠 Overview

This project implements a **text-guided image inpainting system** using the **Stable Diffusion Inpainting Pipeline**.

It enables realistic reconstruction of missing or corrupted image regions by combining:

* Mask-based editing
* Text-conditioned generation
* Context-aware image synthesis

The model generates **high-quality, photorealistic outputs** while preserving surrounding details.

---

## ✨ Key Features

* Text-controlled image generation
* Mask-based region editing
* Semantic understanding using CLIP
* High-quality photorealistic outputs
* GPU-accelerated inference using PyTorch

---

## 🎥 Demo Workflow

1. Upload original image  
2. Upload mask (white = region to edit)  
3. Enter prompt  
4. Run model  
5. Get inpainted output  

---

## 🏗️ Model Architecture

* Stable Diffusion Inpainting Pipeline (`runwayml/stable-diffusion-inpainting`)
* CLIP Text Encoder
* U-Net (generation)
* VAE (encoding & decoding)

---
## 🔬 Technical Insight

This project uses a **Latent Diffusion Model (LDM)**, which operates in a compressed latent space instead of pixel space.

Advantages:
- Faster computation  
- Lower memory usage  
- High-quality generation  

Classifier-Free Guidance (CFG) is used to control how strongly the output follows the text prompt.

## 📊 Sample Output

<p align="center">
  <img src="sample_outputs/input.png" width="220"/>
  <img src="sample_outputs/mask.png" width="220"/>
  <img src="sample_outputs/output.png" width="220"/>
</p>

<p align="center">
  <b>Original</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <b>Mask</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <b>Output</b>
</p>

---

## 🛠️ Tech Stack

* Python
* PyTorch
* Hugging Face Diffusers
* Transformers
* Pillow (PIL)
* Google Colab

---

## 📌 Key Parameters

| Parameter       | Value |
| --------------- | ----- |
| Guidance Scale  | 7.5   |
| Inference Steps | 50    |
| Seed            | 42    |

---

## ⚠️ Note

GitHub may not display the notebook properly due to rendering limitations.

👉 Please use the **"Open in Colab"** button above to view and run the notebook.

## ▶️ Installation

pip install diffusers transformers accelerate torch torchvision pillow

---

## 💡 Example Prompt

photorealistic restoration, high quality, detailed, natural lighting

---

## 💡 Why This Project

This project demonstrates the power of **Generative AI** in image restoration and editing using **Latent Diffusion Models**.

---

## 📈 Results

The model successfully:
- Removes artifacts and noise  
- Maintains texture consistency  
- Generates semantically meaningful content  

The output is both visually realistic and context-aware.
## 🚀 Future Scope

- Integrate Segment Anything Model (SAM) for automatic masking  
- Upgrade to Stable Diffusion XL  
- Build a web interface using Streamlit  
- Add real-time editing capability  

---

## 👩‍💻 Author

**Anna Angel Raju**
