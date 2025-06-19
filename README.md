# Cloth Segmentation with UNet

This project implements a **cloth segmentation model** using a customized **UNet architecture** in PyTorch. It takes an image of a person and segments the clothing region in binary mask format. This is useful for tasks like virtual try-on, e-commerce, or fashion AI systems.

---

## Features

- Custom `UNet` implementation from scratch.
- PyTorch `Dataset` class to load paired images and masks.
- Training and validation loops with:
  - BCEWithLogits loss
  - Dice score metric
  - Pixel-wise accuracy
- Saving predicted masks as images during validation.
- Checkpointing to resume training.

---

## Dataset Structure

The dataset should consist of images and their corresponding binary masks.

dataset/

├── images/

│ ├── 0001.jpg

│ ├── 0002.jpg

│ └── ...

├── masks/

│ ├── 0001.jpg

│ ├── 0002.jpg

│ └── ...
