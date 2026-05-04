# Lab 9 - Morphological Operations

## Overview

This notebook demonstrates basic **morphological image processing operations** using **OpenCV** in Python.
Morphological operations are commonly used in image preprocessing to remove noise, separate objects, and enhance binary images.

## Operations Included

* **Erosion**
* **Dilation**
* **Opening**
* **Closing**

## Technologies Used

* Python 3
* OpenCV (`cv2`)
* NumPy
* Matplotlib

## Files Required

Make sure the following image files are in the same directory as the notebook:

* `Erosion.jpg`
* `Open_Closing.jpg`
* `Opening2.jpg`

## How It Works

### 1. Erosion

Shrinks white regions in a binary image.
Useful for removing small white noise.

### 2. Dilation

Expands white regions in a binary image.
Useful for filling small holes.

### 3. Opening

Combination of:
Erosion → Dilation

Used to remove noise while preserving object shape.

### 4. Closing

Combination of:
Dilation → Erosion

Used to close small holes inside foreground objects.

## Running the Notebook

1. Install dependencies:

```bash
pip install opencv-python numpy matplotlib
```

2. Open the notebook:

```bash
jupyter notebook
```

3. Run all cells sequentially.

## Learning Objectives

By completing this lab, you will learn how to:

* Apply morphological transformations to binary images
* Use structuring elements (kernels)
* Compare effects of different morphological operations
* Preprocess images for computer vision tasks

## Author

Prepared for Image Processing Lab – Morphological Operations
