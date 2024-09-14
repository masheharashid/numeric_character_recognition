# Numeric Character Recognition (NCR)

The project is based on the Kaggle competition, **Numeric Character Recognition**, which involves taking images of handwritten single digits from the MNIST dataset and determining the digit in each image using classification algorithms. Please visit the [competition page](https://www.kaggle.com/competitions/ncr) for the full details and competition rules. 

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Running the Notebook](#running-the-notebook)
- [Running on Google Colab](#running-on-google-colab)
- [Citation](#citiation)

## Project Overview

The objective is to correctly identify digits from the MNIST ("Modified National Institute of Standards and Technology") dataset, which contains handwritten images, using a Convolutional Neural Network (CNN) to achieve the highest categorization accuracy, or the proportion of test images that are correctly classified. 

### File Descriptions

#### 1. `ncr_final_version.ipynb`
This Jupyter notebook contains the implementation of the CNN for classifying MNIST handwritten digits. It includes data preprocessing, model training, evaluation, and visualization of results.

#### 2. `ncr/`
This directory contains training and testing datasets and the submission file for the competition. It includes:
  - `train.csv`: Gray-scale training images of hand-drawn digits with labels (0-9). Each image is 28 x 28 pixels, with pixel values ranging from 0 (light) to 255 (dark).
  - `test.csv`: Same as the training set, but without the label column
  - `sample_submission.csv`: Contains 28,000 lines, one for each image in the test set, with two columns: `ImageId` and `Label` (predicted digit)

#### 3. `final_results.csv`
This file contains the predicted digits for each test image (`test.csv`), following the format of `sample_submission.csv`. 

## Installation 

1. Clone the repository to your local machine:
  ```bash
  git clone https://github.com/masheharashid/numeric_character_recognition.git
  cd numeric_character_recognition
  ```

## Running the Notebook

1. **Launch the Jupyter Notebook Interface**
- Open the terminal and navigate to the project directory. Then, launch the Jupyter Notebook interface and open the Python notebook file

   ```bash
  jupyter notebook ncr_final_version.ipynb
  ```
   
2. Follow the instructions in the notebook and run each cell in order

## Running on Google Colab

**Option 1**:
- Click on the "Open in Colab" button at the top of the `ncr_final_version.ipynb` file or go to this [link](https://colab.research.google.com/github/masheharashid/numeric_character_recognition/blob/master/ncr_final_version.ipynb)

**Option 2**: 
1. Upload the Notebook
- Open [Google Colab](https://colab.google/)
- Upload the `ncr_final_version.ipynb` file

2. **Mount the Google Drive (Optional)**
- If the NCR files are stored in Google Drive, mount the drive to access them:

    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```

3. **Run the Notebook**
- Execute the cells in order as instructed in the notebook

## Citation 

Akaash Tripathi. (2024). Numeric Character Recognition (NCR). Kaggle. https://kaggle.com/competitions/ncr

  
