# Basics Programming in Python (Lap1)

This repository contains a **complete beginner-level introduction to Python programming** implemented in a Jupyter Notebook titled:

📘 **Basics_Programming_Python.ipynb**

The notebook explains Python concepts step by step and demonstrates them using executable code cells.  
It is designed for **students who are new to programming** and want to understand Python fundamentals clearly and practically.

---

## 📌 Purpose of This Notebook

The goal of this notebook is to:
- Teach Python from scratch
- Explain programming concepts using simple examples
- Help students understand how Python code behaves by running it
- Build a foundation for more advanced topics such as data analysis, AI, and machine learning

---

## 🧠 What This Notebook Explains (Detailed)

### 1️⃣ Introduction to Python
- What Python is and why it is popular
- Why Python is used in:
  - Software development
  - Artificial Intelligence
  - Data Science
  - Automation
- How Python code is written and executed in Jupyter Notebook

---

### 2️⃣ Python Syntax Basics
- How Python statements are written
- Importance of indentation in Python
- Difference between Python and other languages (no semicolons, no braces)
- Running simple Python commands

Example concepts:
```python
print("Hello World")

{End of Lap 1}

Image Sampling, Quantization, and Image Operations(Lap2)

This project demonstrates basic image processing techniques using Python, including:

Image sampling (downsampling)

Image quantization (reducing gray levels)

Image addition

Image union using bitwise OR

The implementation uses OpenCV, NumPy, Matplotlib, and Pillow (PIL).

Features
1. Image Sampling

Reduces the spatial resolution of an image by a given factor using nearest-neighbor interpolation.

2. Image Quantization

Reduces the number of grayscale intensity levels in an image.

3. Image Visualization

Displays:

Original image

Sampled image

Quantized image

Side by side using Matplotlib.

4. Image Addition

Adds two grayscale images pixel-by-pixel after resizing them to the same dimensions.

5. Image Union (Bitwise OR)

Performs a union operation between two images using the bitwise OR operator.

Required Libraries

Make sure you have the following Python libraries installed:

pip install opencv-python numpy matplotlib pillow

Input Images

Place the following images in the project directory:

lena_gray_512.tif

cameraman.tif

a.JPG

b.JPG

How the Code Works
Sampling Parameters
sampling_factor = 14


Higher value → more downsampling → lower resolution.

Quantization Parameters
quantization_levels = 9


Fewer levels → more visible intensity steps.

Functions Overview
sample_image(image, factor)

Downsamples the image by the given factor.

quantize_image(image, levels)

Reduces grayscale levels in the image.

plot_images(original, sampled, quantized)

Displays original, sampled, and quantized images.

Output

A figure showing:

Original Image

Sampled Image

Quantized Image

A new image created by adding two images

A new image created by bitwise union of two images

Notes

Images are resized to 400 × 400 before addition or union to ensure matching dimensions.

Bitwise OR is useful for combining image features or masks.

Image addition may overflow; results are cast to uint8.
