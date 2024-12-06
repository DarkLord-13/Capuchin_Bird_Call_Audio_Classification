# Capuchin Bird Audio Classification

This project aims to classify audio clips of Capuchin bird calls using deep learning techniques. The audio data is processed and converted into spectrograms for image classification.

## Project Overview

The project follows these main steps:
1. **Data Preparation**:
    - Install necessary packages.
    - Download the dataset from Kaggle.
    - Extract and preprocess the dataset.
2. **Audio Processing**:
    - Load and preprocess audio files.
    - Convert audio files into spectrograms.
3. **Data Partitioning**:
    - Create TensorFlow datasets for positive (Capuchin bird) and negative (non-Capuchin bird) samples.
    - Split the dataset into training and testing partitions.
4. **Model Building**:
    - Build and compile a deep learning model using TensorFlow and Keras.
5. **Model Training**:
    - Train the model on the training dataset.
    - Evaluate the model on the testing dataset.

## Dependencies

The project requires the following dependencies:
- Python 3.x
- Jupyter Notebook
- TensorFlow
- TensorFlow-IO
- Matplotlib
- Kaggle API

## Installation

1. Clone this repository:
    ```sh
    git clone https://github.com/DarkLord-13/Machine-Learning-01.git
    ```

2. Navigate to the project directory:
    ```sh
    cd Machine-Learning-01
    ```

3. Install the required packages:
    ```sh
    pip install tensorflow tensorflow-gpu tensorflow-io matplotlib kaggle
    ```

4. Download the dataset from Kaggle:
    - Place your `kaggle.json` file in the project directory.
    - Run the following commands to set up the Kaggle API and download the dataset:
    ```sh
    mkdir -p ~/.kaggle
    cp kaggle.json ~/.kaggle/
    chmod 600 ~/.kaggle/kaggle.json
    kaggle datasets download -d kenjee/z-by-hp-unlocked-challenge-3-signal-processing
    ```

5. Extract the dataset:
    ```sh
    unzip z-by-hp-unlocked-challenge-3-signal-processing.zip
    ```

## Usage

Open the Jupyter Notebook `CapuchinBirdAudioClassification.ipynb` and run the cells to execute the project steps.

```sh
jupyter notebook CapuchinBirdAudioClassification.ipynb
