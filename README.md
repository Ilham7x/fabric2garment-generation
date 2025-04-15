# 👗 fabric2garment-generation

**GenAI-Driven Image Generation Pipeline for Sustainable Garment Design and Waste Reduction in Fashion Production**

This repository supports an ongoing research project focused on applying Generative AI to assist sustainable fashion design workflows. It currently contains a custom dataset of fabric screenshots used for conditioning garment generation models. Future updates will include implementation code, ComfyUI workflows, and evaluation scripts.

--

## 📁 Dataset Overview

The `fabric_images/` folder contains **10 preprocessed fabric images**, which were used as conditioning inputs for the garment generation pipeline. These images were extracted from product thumbnails in the [Fashion Product Images Dataset (Kaggle)](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset) and carefully curated for texture clarity.

### Image Preprocessing

All fabric images have been:
- **Resized to 512×512 pixels** using **LANCZOS interpolation** for optimal texture fidelity.
- **Saved as high-quality PNG files**.
- Renamed using a consistent format: `fabric_01.png` to `fabric_10.png`.

These preprocessed images were used in a **Stable Diffusion 1.5-based pipeline** implemented via **ComfyUI**, conditioned by both fabric image input and simple text prompts (e.g., “a floral dress made from this fabric”).

--

## Project Objective

This research explores how GenAI models can reduce textile waste by:
- **Generating realistic garment visuals** using digital fabric inputs.
- **Minimizing the need for physical sampling**, which contributes significantly to pre-consumer waste in fashion production.
- Empowering designers with **creative, low-waste prototyping tools**.

--

## Future Repository Updates

This repository will be expanded to include:
- 📦 ComfyUI node workflow configuration files
- 🧪 Quantitative evaluation scripts (FID, KID, SSIM, LPIPS, CLIP-S)
- 🧵 LoRA integration examples and prompt formatting
- 🛠️ Full source code for the image generation pipeline

---

## 📚 Citation

If you reference this repository or dataset in your work, please cite as:

```
Ilham Ghori. "GenAI-Driven Image Generation Pipeline for Sustainable Garment Design and Waste Reduction in Fashion Production." Research project, 2025. (Unpublished)
```
