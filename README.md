# SUIM Dataset Installation and Notebook Execution Guide

This guide provides instructions on how to install the SUIM dataset and run the associated Jupyter notebook. 

The SUIM dataset is a Segmentation of Underwater IMagery (SUIM) dataset that contains ~1500 images with pixel annotations for eight object categories. <br>
The images have been collected during oceanic explorations and human-robot collaborative experiments, and annotated by 7 human participants.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- Python
- Jupyter Notebook

## Installation

Clone the repository to your local machine:

   ```bash
   git clone https://github.com/loomkoom/suim-segmentation.git
   ```
Change into the project directory:

   ```bash
cd suim-segmentation
   ```
Install the required dependencies:

   ```bash
pip install -r requirements.txt
   ```

## Usage
Download the SUIM dataset at: https://drive.google.com/drive/folders/10KMK0rNB43V2g30NcA1RYipL535DuZ-h

Extract the zip folders, `train_val` is training/validation data and `test` is the test data

change the `ddir` variable at the top of the notebook to point at the folder where you unzipped the training and test folders.

`project_start` has all the data exploration, preparation and training of models up to the Convolution Neural Network. (Notebook cells with !! in front of them are needed, other cells are optional)

`project_models` contains all the previous models with the addittion the construction of the dataset and training of the fully connected CNN's

`project_masks` contains the code to show prediction masks on full images and has some comparisons






