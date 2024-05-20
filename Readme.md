# Filter Multidimensional Signal Using Fourier Transform

This repository contains a comprehensive toolkit for image processing and denoising. It leverages Fourier transformations, various filtering techniques, and calculates error metrics such as PSNR (Peak Signal-to-Noise Ratio) and SSIM (Structural Similarity Index). This toolkit demonstrates practical applications in image denoising using the Smartphone Imaging Denoise Dataset (SIDD) and on individual large and small images for testing purposes.

**Programming Language and Version**
Language: Python
Version: 3.8 or higher
Editor: Visual Studio Code(prefered)

# Setup and Installation
**Prerequisites**
Ensure that Python 3.8+ is installed on your system. If not, you can download it from the official Python website.

**Setting Up a Virtual Environment**
It's recommended to use a virtual environment for Python projects to manage dependencies effectively. You can set up a virtual environment by running the following commands:

In bash run the below code:
```
python -m venv myenv
```


**Activate the virtual environment with:**
*Windows:*
In bash run the below code:
```
myenv\Scripts\activate
```
*macOS and Linux:*
In bash run the below code
```
source myenv/bin/activate
```
**Install the required packages:**
You can install the necessary Python packages using the following commands:
In your bash run any one of the below lines
```
pip install numpy scipy matplotlib skimage opencv-python
```
                
```
pip install -r requirements.txt
```

# Repository Structure
This repository includes two Jupyter notebooks, each serving distinct purposes but implementing the same algorithms and functions:

Denoising_SIDD.ipynb: This notebook applies our denoising algorithm to all images in the SIDD dataset. Note that processing the entire dataset may take approximately 3-4 hours.

Testing_file.ipynb: This notebook is used for testing our functions and algorithms on a single large-sized and a small-sized image.

# Execution Instructions for Jupyter Notebook:
Running Notebooks
To run the Jupyter Notebooks after installation, use the following command:

In bash run the below code
```
jupyter notebook
```

Navigate to the notebook file in the browser that opens up and run the cells.

**For Denoising_SIDD.ipynb:**

It is recommended to not execute this file if you just want to see the outputs as, we uploaded the file after executing and you can see the results just by scrolling down throughout the Denoising_SIDD.ipynb file, instead of executing and waiting for 3-4 hours to view the same results.but if you want to execute follow the command below

Execute all cells in the notebook to process the dataset. You can run all cells by selecting Kernel > Restart & Run All in the Jupyter interface.

**For Testing_file.ipynb:**
Execute all cells in the notebook to process the individual images. You can run all cells by selecting Kernel > Restart & Run All in the Jupyter interface. 

# Execution Time for Testing_file.ipynb file:

Large Image: Approximately 3-4 minutes
Small Image: Approximately 5-7 seconds

**Custom Testing**
Replace the below paths with your ground truth and noisy image paths as shown below for custom testing
```
gt_image = cv2.imread('path_to_your_image/GT_SRGB_010.PNG')
noisy_image = cv2.imread('path_to_your_image/GT_SRGB_010.PNG')
```
# Notes

*Note1:* Two code files are included in this repository. Although they implement the same functions and algorithms, they serve different purposes as outlined.

*Note2:* Processing times may vary based on system performance and image complexity.



