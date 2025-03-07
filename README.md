Image Generation Using ComfyUI and Stable Diffusion
This repository explores Stable Diffusion, a powerful AI model for generating high-quality images, and ComfyUI, a modular, node-based interface that enhances control and customization.

Table of Contents
Introduction
Features
Requirements
Installation
Usage
Introduction
Stable Diffusion is an advanced deep learning model capable of generating high-quality images from textual descriptions. However, interacting with it through code can be complex. ComfyUI simplifies this process by offering a visual programming environment where users can design custom image generation workflows without coding.

This project combines Stable Diffusion with ComfyUI, providing a user-friendly and highly customizable experience for AI-driven image creation.

Features
✅ Visual Workflow Design – Easily build complex image generation pipelines with ComfyUI's node-based interface.
✅ Text-to-Image Generation – Convert textual descriptions into stunning images using Stable Diffusion.
✅ Customizable Parameters – Fine-tune parameters like resolution, sampling methods, and noise levels for better artistic control.
✅ Modular Design – Add, remove, or rearrange nodes in ComfyUI to experiment with different image processing techniques.
✅ Real-Time Feedback (if supported) – Get previews of generated images as you tweak parameters.
✅ Extensible with Custom Scripts – Integrate Python scripts and custom nodes for advanced functionalities.

Requirements
3.2.1 Hardware Requirements
Operating System: Windows 10/11, macOS, or Linux (Linux recommended for performance)
Processor (CPU): Multi-core modern processor (Intel i5/Ryzen 5 or higher)
Graphics Card (GPU): NVIDIA GPU with at least 8GB VRAM (Recommended: RTX 3060+ or equivalent)
Memory (RAM): Minimum 16GB (Recommended: 32GB+ for optimal performance)
Storage: SSD with at least 20GB free space
3.2.2 Software Requirements
Python: Version 3.8+ (Recommended: 3.10 or 3.11)
ComfyUI: Download from the official repository
Stable Diffusion Model Checkpoint: (e.g., .ckpt or .safetensors from Hugging Face)
Required Python Libraries (Install via pip):
bash
Copy
Edit
pip install torch torchvision torchaudio transformers numpy Pillow Flask requests tqdm filelock gradio omegaconf
CUDA (For NVIDIA GPUs): Ensure PyTorch is installed with the correct CUDA version
Installation
Step 1: Install Python
Ensure Python 3.8 or higher is installed (recommended: 3.10 or 3.11).

Step 2: Install ComfyUI
Clone the ComfyUI repository and follow the setup instructions. Example:

bash
Copy
Edit
git clone https://github.com/comfyanonymous/ComfyUI.git
cd ComfyUI
Step 3: Download the Stable Diffusion Model
Obtain the v1-5-pruned-emaonly-fp16 model from Hugging Face and place it in:

bash
Copy
Edit
ComfyUI_windows_portable/ComfyUI/models/checkpoints
(This is necessary for ComfyUI to detect the model automatically.)

Step 4: Install Dependencies
Navigate to the ComfyUI directory and set up a virtual environment (recommended):

bash
Copy
Edit
python3 -m venv .venv   # Create a virtual environment  
source .venv/bin/activate   # Activate (Linux/macOS)  
.venv\Scripts\activate   # Activate (Windows)  
Then, install the required Python libraries:

bash
Copy
Edit
pip install torch torchvision torchaudio transformers numpy Pillow Flask requests tqdm filelock gradio omegaconf
(Ensure PyTorch is installed with the correct CUDA version for GPU acceleration.)

Step 5: Run ComfyUI
Launch ComfyUI by running:

bash
Copy
Edit
python main.py
Once loaded, ComfyUI should automatically detect the Stable Diffusion model.

Usage
Start ComfyUI – Run ComfyUI according to its documentation.
Load Workflow (Optional) – Use a pre-designed workflow or create a new one.
Enter Prompt – Input your text prompt in the designated ComfyUI node.
Adjust Parameters – Modify sampling methods, resolution, and other settings.
Generate Image – Execute the workflow to generate an image.
View & Save Results – The generated image will be displayed in ComfyUI, ready for further refinement.
