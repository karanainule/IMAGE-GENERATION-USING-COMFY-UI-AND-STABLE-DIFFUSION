# Image Generation Using ComfyUI and Stable Diffusion

This repository explores **Stable Diffusion**, a powerful AI model for generating high-quality images, and **ComfyUI**, a modular node-based interface that provides enhanced control and customization for image generation.

## Table of Contents

- [Introduction](#introduction)
- [Key Features](#key-features)
- [System Requirements](#system-requirements)
- [Installation Guide](#installation-guide)
- [Usage Instructions](#usage-instructions)

## Introduction

Stable Diffusion is an advanced deep-learning model capable of generating stunning images based on textual prompts. **ComfyUI** simplifies the interaction with Stable Diffusion by offering a **visual workflow builder**, allowing users to craft and fine-tune image generation pipelines without deep programming knowledge. 

This project leverages both technologies to create a **seamless and flexible** image generation experience tailored to individual needs.

## Key Features

- **Intuitive Node-Based Workflow:** Utilize ComfyUI's modular interface to construct sophisticated image generation pipelines effortlessly.
- **Text-to-Image Conversion:** Generate unique images by providing descriptive text inputs.
- **Customizable Parameters:** Fine-tune model parameters within ComfyUI to achieve different artistic styles and output variations.
- **Modular and Scalable:** Add, remove, or rearrange nodes in the workflow to experiment with diverse processing techniques.
- **Real-time Feedback:** (Depending on ComfyUI's capabilities) Preview intermediate results to refine image outputs efficiently.
- **Extensibility with Custom Scripts:** Enhance functionality by integrating custom Python scripts within ComfyUI.

## System Requirements

### Hardware
- **Operating System:** Windows 10/11, macOS, or Linux (recommended for optimal performance).
- **Processor (CPU):** Multi-core modern processor.
- **Graphics Card (GPU):** NVIDIA GPU with at least 8GB VRAM (12GB+ recommended). AMD GPUs may require additional configuration.
- **Memory (RAM):** Minimum 16GB (32GB+ recommended for large models).
- **Storage:** High-speed SSD with sufficient free space.

### Software
- **Python 3.8+** (Recommended: 3.10 or 3.11).
- **ComfyUI** (Download from the official repository).
- **Stable Diffusion Model Checkpoint** (Ensure compatibility with ComfyUI, e.g., `.ckpt` or `.safetensors`).
- **Required Python Libraries** (Install via `pip`):
  ```bash
  pip install torch torchvision torchaudio transformers numpy Pillow Flask requests tqdm filelock gradio omegaconf
  ```
  *(Ensure PyTorch is installed with the appropriate CUDA version for NVIDIA GPUs.)*

## Installation Guide

1. **Install Python**: Ensure Python 3.8 or higher is installed (3.10/3.11 recommended).
2. **Clone ComfyUI Repository**:
   ```bash
   git clone <ComfyUI-repo-link>
   cd ComfyUI
   ```
3. **Download Stable Diffusion Model**: Retrieve a compatible model checkpoint (e.g., `v1-5-pruned-emaonly-fp16`) from **Hugging Face** or another trusted source.
4. **Move Model File**: Place the downloaded model in:
   ```bash
   ComfyUI/models/checkpoints/
   ```
5. **Set Up Virtual Environment (Recommended):**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # macOS/Linux
   .venv\Scripts\activate  # Windows
   ```
6. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
7. **Launch ComfyUI**:
   ```bash
   python main.py
   ```

## Usage Instructions

1. **Start ComfyUI**: Run ComfyUI according to its official documentation.
2. **Load or Create a Workflow**: Import an existing workflow or design a custom pipeline.
3. **Input a Prompt**: Enter a descriptive text prompt in the appropriate ComfyUI node.
4. **Adjust Parameters**: Modify node settings to refine the output.
5. **Generate an Image**: Execute the workflow and generate the image.
6. **Review and Save Output**: The generated image will appear in the ComfyUI interface.

---

