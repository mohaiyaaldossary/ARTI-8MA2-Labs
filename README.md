Basics of Programming with Python(lap1)


📋 Contents
TaskDescriptionSetupInstalling Anaconda, Jupyter, and SpyderNumPy ExercisesArray creation, indexing, and selectionTask 1Core NumPy operations and matrix manipulationTask 2Loading and visualizing images (OpenCV & PIL)Task 3Saving images to diskTask 4Displaying images as NumPy arraysTask 5Saving work via Git

⚙️ Setup
Prerequisites

Anaconda 3 — includes Python, Jupyter, and Spyder out of the box

Installation Steps

Download and install the latest version of Anaconda 3 from anaconda.com
Launch Jupyter Notebook or Spyder from the Anaconda Navigator
Open Basics_Programming_Python.ipynb


📦 Dependencies
The following libraries are used in this notebook:
bashpip install numpy opencv-python pillow matplotlib
LibraryPurposenumpyArray creation and numerical operationsopencv-python (cv2)Image loading and savingPillow (PIL)Image loading, processing, and savingmatplotlibImage visualization and plotting

📚 Topics Covered
NumPy Fundamentals

Importing NumPy
Creating arrays: zeros, ones, arange, linspace
Generating random numbers and arrays (rand, randn)
Creating identity matrices with eye
Reshaping arrays

NumPy Indexing & Selection

Accessing specific elements by index
Extracting rows and columns
Slicing 2D arrays to get sub-arrays

Image Processing with OpenCV & PIL (Tasks 2–4)

Reading images using cv2.imread() and PIL.Image.open()
Visualizing images with matplotlib.pyplot
Saving images to disk with cv2.imwrite() and img.save()
Converting images to NumPy arrays and inspecting their shape


🗂️ File Structure
project/
├── Basics_Programming_Python.ipynb   # Main notebook
├── cameraman.tif                     # Sample image (required for Task 2)
├── lena_gray_512.tif                 # Sample image (required for Task 2)
└── README.md

Note: Update the image file paths in cells for Tasks 2–4 to match your local directory before running.


🚀 Usage

Clone or download this repository
Place the required image files (cameraman.tif, lena_gray_512.tif) in your working directory
Update the file paths in the notebook cells accordingly
Run the notebook cells sequentially from top to bottom


💾 Saving Your Work
After completing the notebook, commit your progress to Git:
bashgit add .
git commit -m "Completed lab1 tutorial"
git push origin master

📖 Resources

NumPy Cheat Sheet (DataCamp)
NumPy Official Docs
OpenCV Python Tutorials
Pillow Documentation
{end of lap 1}
////////////
LAP 2 — Image Sampling, Quantization & Arithmetic Operations
A Jupyter Notebook demonstrating core image processing techniques including spatial downsampling, grayscale quantization, image addition, and bitwise union operations using OpenCV, PIL, NumPy, and Matplotlib.

📋 Contents
SectionDescriptionImage LoadingLoad grayscale images using OpenCV and PILSamplingDownsample an image by a given factor using nearest-neighbor interpolationQuantizationReduce the number of grayscale intensity levelsVisualizationSide-by-side display of original, sampled, and quantized imagesImage AdditionAdd two images pixel-by-pixel using NumPy arraysBitwise UnionPerform bitwise OR between two images

⚙️ Setup
Prerequisites

Python 3.x
Anaconda (recommended) or a standard Python environment with pip

Installation
Install the required libraries:
bashpip install numpy opencv-python pillow matplotlib

📦 Dependencies
LibraryPurposenumpyArray operations and pixel-level arithmeticopencv-python (cv2)Grayscale image loading and resizingPillow (PIL)Image loading, resizing, and displaymatplotlibImage visualization and subplot rendering

🗂️ Required Image Files
The following image files must be present in the same directory as the notebook:
FileUsed Inlena_gray_512.tifSampling, Quantization, and Image Additioncameraman.tifImage Additiona.JPGBitwise Unionb.JPGBitwise Union

Note: All images are resized to 400×400 pixels before arithmetic operations to ensure compatible array dimensions.


📚 Topics Covered
1. Spatial Sampling (sample_image)
Downsamples an image by an integer factor using cv2.resize() with nearest-neighbor interpolation.
pythonsampled_image = sample_image(original_image, factor=14)
2. Grayscale Quantization (quantize_image)
Reduces the number of intensity levels in an image by grouping pixel values into discrete steps.
pythonquantized_image = quantize_image(original_image, levels=9)
3. Image Visualization (plot_images)
Displays the original, sampled, and quantized images side by side using Matplotlib subplots.
4. Image Addition
Adds two grayscale images pixel-by-pixel by converting them to NumPy arrays.
pythonaddition = im1arr + im2arr

⚠️ Raw addition may cause pixel overflow beyond 255. Consider using np.clip() or cv2.add() for overflow-safe addition.

5. Bitwise Union (OR)
Performs a bitwise OR between two images, combining their bright regions.
pythonunion = im3arr | im4arr

🚀 Usage

Place all required image files in the same directory as LAP_2.ipynb
Launch Jupyter Notebook:

bash   jupyter notebook LAP_2.ipynb

Run all cells sequentially from top to bottom


🗂️ File Structure
project/
├── LAP_2.ipynb          # Main notebook
├── lena_gray_512.tif    # Grayscale test image
├── cameraman.tif        # Grayscale test image
├── a.JPG                # Custom image for bitwise operation
├── b.JPG                # Custom image for bitwise operation
└── README.md
