# Digital Image Processing using OpenCV

## Overview
This project demonstrates basic concepts of digital image processing using **Python** and **OpenCV**.

A digital image is represented as a matrix of pixel values:
- Grayscale image → each pixel has one intensity value (0–255)
- Color image → each pixel has three values (RGB)

By applying mathematical operations to these values, we can enhance, analyze, and transform images.

---

## Objectives
- Understand digital image representation
- Apply geometric transformations
- Apply intensity transformations
- Enhance image visibility and contrast
- Practice image manipulation using OpenCV

---

## Tools Used
- Python 3
- OpenCV (cv2)
- NumPy

---

## Implemented Operations

### 1. Geometric Transformations
Operations that change image position or shape without changing meaning of pixel intensity.

Examples:
- Resize (Scaling)
- Rotation
- Shearing

**Purpose:** Adjust orientation and perspective of the image.

---

### 2. Intensity Transformations
Operations that modify brightness values of pixels.

Examples:
- Negative Transformation
- Log Transformation
- Power-Law (Gamma Correction)

**Purpose:** Improve visibility and reveal hidden details.

---

## How to Run

1. Install required libraries:
```bash
pip install opencv-python numpy
