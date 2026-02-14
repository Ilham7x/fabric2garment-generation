# 👗 fabric2garment-generation

**GenAI-Driven Image Generation Pipeline for Sustainable Garment Design and Waste Reduction in Fashion Production**

This repository supports a research project focused on using Generative AI to assist sustainable fashion design. It includes a curated fabric dataset, a ComfyUI-based image generation pipeline, and evaluation notebooks for assessing model performance.

---

## 📁 Dataset Overview

The `fabric_images/` folder contains **10 preprocessed fabric images**, which were used as conditioning inputs for the garment generation pipeline. These images were extracted from product thumbnails in the [Fashion Product Images Dataset (Kaggle)](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset) and carefully curated for texture clarity.

### Image Preprocessing

All fabric images have been:
- Resized to 512×512 pixels using LANCZOS interpolation for optimal texture fidelity.
- Saved as high-quality PNG files.
- Renamed using a consistent format: `fabric_01.png` to `fabric_10.png`.

These preprocessed images were used in a Stable Diffusion 1.5-based pipeline implemented via ComfyUI, conditioned by both fabric image input and simple text prompts (e.g., “a floral dress made from this fabric”).

---

## ⚙️ ComfyUI Implementation

The notebook `ComfyUI_Pipeline.ipynb` contains:
- An overview of the ComfyUI-based workflow using LoRA-enhanced Stable Diffusion 1.5.
- The model setup with fixed parameters: **CFG = 8**, **Steps = 50**, **Denoise = 0.85**, **Sampler = Euler**, **Seed = 2024**.
---

## 📊 Evaluation Metrics

The notebook `Evaluation_Metrics.ipynb` contains:
- Metric definitions and calculation code for:
  - **FID**
  - **KID**
  - **SSIM**
  - **LPIPS**
  - **CLIP-S**
- Comparison of results from three diffusion models: **DreamShaper v8**, **Realistic Vision v5.1**, and **MajicMix v5**.
---

## 🎯 Project Objective

This research explores how GenAI models can reduce textile waste by:
- **Generating realistic garment visuals** using digital fabric inputs.
- **Minimizing the need for physical sampling**, which contributes significantly to pre-consumer waste in fashion production.
- Empowering designers with **creative, low-waste prototyping tools**.

---
## 📄 Publication

This work was presented at the AAAI Summer Symposium Series 2025 (SuSS-25) — Human-AI Collaboration Symposium.
Paper: [View PDF]((https://ojs.aaai.org/index.php/AAAI-SS/article/view/36056/38211))

---

## 📚 Citation

If you reference this repository or dataset in your work, please cite as:

```
Ghori, I., Karim, K., & Alkawadri, D. (2025).
GenAI-Driven Image Generation Pipeline for Sustainable Garment Design and Waste Reduction in Fashion Production.
Presented at the AAAI Human-AI Collaboration Symposium (AAAI SuSS-25).
```
