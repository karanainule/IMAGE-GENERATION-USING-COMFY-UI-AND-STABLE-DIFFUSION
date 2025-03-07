# IMAGE-GENERATION-USING-COMFY-UI-AND-STABLE-DIFFUSION

This repository explores Stable Diffusion, a powerful AI model for generating high-quality images, and ComfyUI, a modular node-based interface that enhances control and customization.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)

## Introduction

Stable Diffusion is a powerful deep learning model capable of generating high-quality images from textual descriptions. ComfyUI simplifies the interaction with Stable Diffusion by providing a visual programming environment where users can create custom image generation pipelines. This project combines these two tools to offer a user-friendly and highly customizable image generation experience.

## Features

*   **Visual Workflow Design:** Create complex image generation pipelines using ComfyUI's node-based interface.
*   **Text-to-Image Generation:** Generate images from textual descriptions using Stable Diffusion.
*   **Customizable Parameters:** Fine-tune image generation parameters within ComfyUI to achieve specific artistic styles and results.
*   **Modular Design:** Easily add, remove, or rearrange nodes in ComfyUI to experiment with different image processing techniques.
*   **Real-time Feedback:**  (Potentially, depending on ComfyUI features) Observe previews of generated images as parameters are adjusted, accelerating the creative process.
*   **Extensible with Custom Scripts:** Integrate custom Python scripts and nodes into ComfyUI for advanced functionalities.

## Requirements

### Hardware

*   Operating System: Windows 10/11, macOS, or a Linux distribution (Linux recommended for performance).
*   Processor (CPU): Modern multi-core CPU.
*   Graphics Card (GPU): NVIDIA GPU with at least 8GB VRAM (12GB+ recommended).  AMD GPUs are supported but may require specific configuration and might have lower performance.
*   Memory (RAM): 16GB RAM minimum (32GB+ recommended).
*   Storage: Fast SSD with ample storage space.

### Software

*   Python 3.8+ (3.10 or 3.11 recommended).
*   ComfyUI (Download and install from the official repository).
*   Stable Diffusion Model Checkpoint (Download a compatible model file, e.g., `.ckpt` or `.safetensors`).
*   Python Libraries (Install using `pip`):
    *   `torch torchvision torchaudio` (for PyTorch)
    *   `transformers`
    *   `numpy`
    *   `Pillow`
    *   `Flask` (if using a web interface)
    *   `requests`
    *   `tqdm`
    *   `filelock`
    *   `gradio` (if using Gradio interface)
    *   `omegaconf`

## Installation
Install Python: Ensure you have Python 3.8 or higher installed. (3.10 or 3.11 are recommended).

Install ComfyUI:  ComfyUI was deployed locally using the GitHub repository.  Clone the repository to your desired location. (Provide the repository link if applicable).  Follow any specific instructions in the repository for initial setup.

Download Stable Diffusion Model: The v1-5-pruned-emaonly-fp16 model was downloaded from Hugging Face. (Provide the Hugging Face model link if possible).

Place Model Checkpoint: The downloaded model file (v1-5-pruned-emaonly-fp16) was placed in the following directory within the ComfyUI installation: ComfyUI_windows_portable\ComfyUI\models\checkpoints.  This specific location is crucial as it's where ComfyUI looks for model files during initialization.

Install Dependencies: Open a terminal or command prompt, navigate to your ComfyUI directory, and create a virtual environment (recommended):

Bash

python3 -m venv .venv  # Create a virtual environment
source .venv/bin/activate  # Activate the virtual environment (Linux/macOS)
.venv\Scripts\activate  # Activate the virtual environment (Windows)
Then, install the required Python libraries:

Bash

pip install torch torchvision torchaudio transformers numpy Pillow Flask requests tqdm filelock gradio omegaconf
(Important Note: Ensure that the PyTorch installation matches your CUDA version if you have a compatible NVIDIA GPU.  Refer to the PyTorch installation instructions for specific CUDA versions.)

Run ComfyUI: Launch ComfyUI according to its documentation.  Because the model checkpoint is now in the correct directory, ComfyUI should automatically recognize it upon startup.
    ```

## Usage

1.  **Run ComfyUI:** Launch ComfyUI according to its documentation.
2.  **Load Workflow (Optional):** If you have a pre-designed ComfyUI workflow, load it. Otherwise, you can create a new workflow from scratch.
3.  **Input Prompt:** Enter your text prompt in the appropriate ComfyUI node.
4.  **Adjust Parameters:** Modify the parameters of the various nodes in your workflow to customize the image generation process.
5.  **Generate Image:** Execute the workflow to generate the image.
6.  **View Results:** The generated image will be displayed in ComfyUI.



