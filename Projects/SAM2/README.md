
# Implementing Meta's SAM2 
This repository demonstrates the implementation and usage of Meta's Segment Anything 2 (SAM2) model for image segmentation tasks. The notebook explores different segmentation approaches including automated mask generation and interactive prompting using points and bounding boxes.


# Features 🌟

* Setup and installation of SAM2 and its dependencies
* GPU-accelerated inference with CUDA optimization
* Multiple model size options (tiny to large)
* Automated mask generation with customizable parameters
* Interactive segmentation using:
    * Bounding box prompts
    * Point prompts


* Visualization tools for segmentation results

# Pre-requisites 📈
* CUDA-capable GPU
* Python 3.x
* PyTorch with CUDA support
* OpenCV
* supervision
* jupyter_bbox_widget

# Installation
git clone https://github.com/facebookresearch/segment-anything-2.git

cd segment-anything-2

pip install -e .

pip install supervision jupyter_bbox_widget

# Model Checkpoints
SAM2 is available in four different sizes:

* sam2_hiera_tiny.pt (38.9M parameters)
* sam2_hiera_small.pt
* sam2_hiera_base_plus.pt
* sam2_hiera_large.pt (224.4M parameters)

# Customization
The mask generator can be customized with various parameters:

* points_per_side
* pred_iou_thresh
* stability_score_thresh
* crop_n_layers
* box_nms_thresh

...and more for fine-tuning segmentation results


# Lessons 📝

This implementation requires sufficient GPU memory and CUDA support. The model performance may vary based on the chosen model size and hardware capabilities.

# License
This project follows the license terms of Meta's Segment Anything 2 model.