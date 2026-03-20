🎨 Image Inpainting using Stable Diffusion

"Python" (https://img.shields.io/badge/Python-3.10-blue)
"PyTorch" (https://img.shields.io/badge/PyTorch-DeepLearning-red)
"HuggingFace" (https://img.shields.io/badge/HuggingFace-Diffusers-yellow)
"Status" (https://img.shields.io/badge/Project-Completed-brightgreen)

---

🚀 Run in Colab

""Open In Colab" (https://colab.research.google.com/assets/colab-badge.svg)" (https://colab.research.google.com/drive/132Oeq4rRKaQ6GhblgENZVEoUTP2EXzc2)

---

🧠 Overview

This project implements a text-guided image inpainting system using the Stable Diffusion Inpainting Pipeline.

It enables realistic reconstruction of missing or corrupted image regions by combining:

- 🧩 Mask-based editing
- 🧠 Text-conditioned generation
- 🎯 Context-aware image synthesis

The model generates high-quality, photorealistic outputs while preserving surrounding details.

---

✨ Key Features

- 🎯 Text-controlled image generation
- 🧩 Mask-based region editing
- 🧠 Semantic understanding using CLIP
- 🖼️ High-quality photorealistic outputs
- ⚡ GPU-accelerated inference using PyTorch

---

⚙️ How It Works

1. Upload an original image
2. Upload a mask image (white = area to modify)
3. Provide a text prompt
4. Model generates realistic content in masked region

---

🏗️ Model Architecture

This project uses:

- Stable Diffusion Inpainting Pipeline
  - Model: "runwayml/stable-diffusion-inpainting"
- CLIP Text Encoder → understands prompts
- U-Net → generates missing regions
- VAE → encodes and decodes images

💡 The model operates in a latent space, making it efficient and scalable.

---

📊 Sample Output

<h3 align="center">📊 Image Inpainting Result</h3><p align="center">
  <img src="sample_outputs/input.png" width="220"/>
  <img src="sample_outputs/mask.png" width="220"/>
  <img src="sample_outputs/output.png" width="220"/>
</p><p align="center">
  <b>Original</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <b>Mask</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <b>Output</b>
</p>---

🛠️ Tech Stack

- Python
- PyTorch
- Hugging Face Diffusers
- Transformers
- Pillow (PIL)
- Google Colab (GPU)

---

📌 Key Parameters

Parameter| Value| Description
Guidance Scale| 7.5| Controls prompt adherence
Inference Steps| 50| Quality vs speed trade-off
Seed| 42| Ensures reproducibility

---

▶️ Installation

pip install diffusers transformers accelerate torch torchvision pillow

---

▶️ Usage

- Run the notebook in Google Colab with GPU enabled
- Upload input image and mask
- Modify prompt if needed
- Execute the pipeline to generate results

---

💡 Example Prompt

photorealistic restoration, high quality, detailed, natural lighting

---

⚠️ Notes

- Mask must be black & white
  - White → region to modify
- Recommended resolution: 512 × 512
- GPU recommended for faster execution

---

💡 Why This Project

This project demonstrates the power of Generative AI in:

- Image restoration
- Content editing
- AI-assisted creativity

It showcases practical use of Latent Diffusion Models in real-world applications.

---

🚀 Future Improvements

- Integration with Segment Anything Model (SAM)
- Support for Stable Diffusion XL
- Web interface (Streamlit / Flask)
- Real-time inpainting UI

---

📄 Project Report

Detailed explanation available in:
📄 "report.pdf"

---

👩‍💻 Author

Anna Angel Raju
B.Tech Computer Science

---
