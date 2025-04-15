# fabric2garment-generation

This repository supports the research paper _"GenAI-Driven Image Generation Pipeline for Sustainable Garment Design and Waste Reduction in Fashion Production."_ It contains the custom dataset of fabric screenshots used to condition garment generation models and will later include implementation code and model configurations.

## 📂 Dataset 

This repository includes a folder named fabric_images/, which contains 10 preprocessed fabric images used for garment generation experiments.

🖼️ Image Preprocessing
All fabric images were:
- Resized to 512×512 pixels using LANCZOS interpolation to preserve fabric texture fidelity.
- Saved in PNG format with consistent filenames: fabric_01.png to fabric_10.png.
- These images served as the conditioning input for the ComfyUI-based generation pipeline.

## 🧠 Purpose

This dataset was created to support experimentation in garment generation conditioned on fabric texture and text prompts. The goal is to reduce reliance on physical sampling in fashion design.

## 🔍 Future Updates

This repository will be updated to include:
- ComfyUI workflow configurations
- Quantitative evaluation scripts
- Full generation pipeline code

## 🧾 Citation

If you use this dataset or code, please cite:
**Ilham Ghori**, *GenAI-Driven Image Generation Pipeline for Sustainable Garment Design and Waste Reduction in Fashion Production*, 2025.
