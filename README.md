# SAM2 for Leaf Disease Segmentation

## Leaf Disease Segmentation Dataset

This dataset is designed for the task of segmenting diseased areas on leaf images. It comprises a collection of RGB leaf images and corresponding RGBA segmentation masks, along with a CSV file for easy data handling during model training.  This dataset is also known as the "Leaf Segmentation Dataset SAM2 format" on Kaggle.

**Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/ankanghosh651/leaf-sengmentation-dataset-sam2-format)

### Dataset Structure

The dataset is organized into the following directories:

-   **Images/**: This directory contains 588 RGB images in `.jpg` format (in most cases). These images showcase leaves with various types of diseases.
-   **Masks/**: This directory contains 588 RGBA segmentation masks in `.png` format. Each mask corresponds to an image in the `images/` directory and annotates the diseased regions of the leaves.
-   **train.csv**: This CSV file maps each image file name to its corresponding mask file name. This mapping is crucial for correctly pairing images with their respective ground truth masks during the training process.

### Data Format Details

*   **Images**: Typically `.jpg` format, containing 588 RGB images of leaves.
*   **Masks**: `.png` format, with RGBA channels representing the segmentation of diseased areas.
*   **train.csv**: A comma-separated file with (at least) two columns:
    *   `image_id`: The file name of the image (e.g., `image1.jpg`).
    *   `mask_id`: The file name of the corresponding mask (e.g., `image1.png`).
        *   *Note: the columns name may vary*

### Intended Use

This dataset is ideal for training and evaluating deep learning models for semantic segmentation, specifically for identifying and delineating diseased regions on leaves. It can be used in applications such as:

*   Automated plant disease diagnosis
*   Precision agriculture
*   Development of image-based disease detection systems
## Instructions to install Segment Anything 2 and installing dependencies 

This repository contains the code and resources for **Segment Anything 2** by Facebook Research.

## Installation Instructions

Follow these steps to clone, navigate, and install this repository in editable mode.

### 1. Clone the Repository
To clone this repository, run the following command:
```bash
git clone https://github.com/facebookresearch/segment-anything-2.git

```
### 2. Change Directory
Navigate into the cloned repository:
```bash
cd segment-anything-2
```
### 3. Install Dependencies
Install the repository in editable mode using `pip`:

```bash
pip install -e .
```

