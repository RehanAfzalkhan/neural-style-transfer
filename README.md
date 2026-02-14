# Deep Learning Autoencoder / Style Transfer Project

## Overview

This project implements deep learning image processing models using Python. It includes neural network architectures such as Autoencoders and Neural Style Transfer pipelines using PyTorch / TensorFlow.

The goal of the project is to:

* Learn feature representations of images
* Reconstruct images using encoder–decoder networks
* Transfer artistic style from one image to another
* Run training and inference on GPU

---

## Requirements

Make sure you have:

* Python 3.9 – 3.11
* NVIDIA GPU (recommended)
* CUDA installed (matching PyTorch version)

### Python Libraries

Install dependencies:

```bash
pip install torch torchvision torchaudio
pip install tensorflow keras
pip install pillow numpy matplotlib opencv-python
```

---

## Setup Virtual Environment (Recommended)

```bash
python -m venv nstenv

# Windows
nstenv\Scripts\activate

# Linux / Mac
source nstenv/bin/activate
```

---

## Project Structure

```
project/
│── models/           # neural network architectures
│── images/           # input images (content & style)
│── outputs/          # generated images
│── main.py           # main execution file
│── train.py          # training script (if available)
│── utils.py          # helper functions
│── README.md
```

---

## Run the Project

Place your images inside the project folder:

```
content.png
style.png
```

Then run:

```bash
python main.py
```

The generated image will be saved inside the `outputs/` folder.

---

## GPU Usage Check

To verify GPU is working:

```python
import torch
print(torch.cuda.is_available())
print(torch.cuda.get_device_name(0))
```

If it prints `True`, GPU is enabled.

---

## Notes

* First run may download pretrained VGG weights automatically
* Use smaller image sizes if GPU memory is limited
* Ensure CUDA version matches installed PyTorch build

---

## Git
