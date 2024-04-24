# MRI Geometric Distortion Calculation Algorithm

The developed algorithm aims to automatically calculate geometric distortions in MRI scans. This repository contains the code and documentation related to the development process of the algorithm.

## Overview

The algorithm's development process is detailed in this repository. To enable future studies to utilize the developed algorithm, it has been made publicly available [here](https://github.com/BernardoCampilho/MSc_Thesis_MRI_Distortion).

The code's overall structure can be divided into three main parts:

### Image Registration

While Eclipse, a commercial software, is typically used for image registration in the clinical workflow at IPO-Porto, this study has developed an alternative algorithm to ensure independence from commercial software. This alternative approach addresses the limitation of Eclipse not being open source, which could hinder result reproducibility. However, given the pre-existing integration of Eclipse within IPO-Porto's clinical operations, including direct image transfer between MRI scanners and treatment planning computers, the registration results obtained using Eclipse were used to derive the final outcomes.

### Insert Detection

The algorithm detects inserts on CT and MRI scans separately after preprocessing and filtering the data to ensure only meaningful and accurate blobs are detected as inserts.

### Distortion Calculation

At this stage, after preprocessing steps related to slice thickness and resolution differences between CT and MRI scans, as well as registration application, the geometric distortion is calculated for each matched insert centroid. The results are processed, and visualization tools facilitate the interpretation of the output results.

## Code

The code provided in this repository is written in Python using OpenCV and NumPy libraries for image processing tasks. It includes functionality for:

- Reading MRI images from a specified folder path
- Preprocessing and filtering image data
- Detecting inserts on CT and MRI scans
- Calculating geometric distortion for each matched insert centroid
- Visualizing results

  
## License

This project is licensed under the MIT License.



## Usage

To use the code, simply clone or download this repository and run the provided Python script. Ensure you have the necessary dependencies installed, including OpenCV, NumPy, and matplotlib.

```bash
git clone https://github.com/BernardoCampilho/MRI_Distortion.git
cd MRI_Distortion





