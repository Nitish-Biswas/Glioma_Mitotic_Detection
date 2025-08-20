# Glioma Mitosis Detection

This project contains a Jupyter Notebook for detecting mitosis in glioma histology images. The notebook performs a comprehensive exploratory data analysis (EDA) and then implements and trains one Vision Transformer (ViT-B/16) and four different deep learning models for classification: ConvNeXtSmall, EfficientNetV2B0, ResNet101V2, and DenseNet201.

## Kaggle Competition

This project was developed for the [Glioma-MDC 2025 (ISBI)](https://www.kaggle.com/competitions/UBC-OCEAN) competition on Kaggle.

* **My Kaggle Profile:** [Nitish Biswas](https://www.kaggle.com/nitishbiswas1)
* **Link to My Notebook:** [Vision Transformer](https://www.kaggle.com/code/nitishbiswas1/vision-transformer1/notebook)

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Notebook Structure](#notebook-structure)
- [Models](#models)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Glioma is a type of tumor that occurs in the brain and spinal cord. The presence and frequency of mitotic figures (cells undergoing division) are crucial indicators for grading the aggressiveness of these tumors. This notebook provides a complete workflow for training and evaluating deep learning models to automate the detection of mitosis in glioma histology slides.

## Features

* **Detailed Exploratory Data Analysis (EDA)**: The notebook includes a thorough analysis of the dataset, including class distribution, region of interest (ROI) size, spatial distribution, and image intensity statistics.
* **Multiple Model Implementations**: One Vision Transfomer and Four powerful and modern convolutional neural network (CNN) architectures are implemented for comparison:
    * ViT-B/16
    * ConvNeXtSmall
    * EfficientNetV2B0
    * ResNet101V2
    * DenseNet201
* **End-to-End Workflow**: The notebook covers the entire process from data loading and preprocessing to model training, evaluation, and submission file generation for a Kaggle competition.
* **Custom Data Generator**: A Keras data generator is used to efficiently load and preprocess image patches for training and evaluation.
* **Training and Evaluation**: The models are trained with modern techniques such as AdamW optimizer, learning rate scheduling, and early stopping. The results are visualized with training history plots, classification reports, and confusion matrices.

## Getting Started

### Prerequisites

* Python 3
* Jupyter Notebook or JupyterLab
* Kaggle account and `kaggle.json` API token

### Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/Nitish-Biswas/Glioma_Mitotic_Detection
    cd glioma_mitotic_detection
    ```

## Usage

1.  Open the `Glioma_detection.ipynb` notebook in Jupyter or your preferred environment.
2.  When prompted, upload your `kaggle.json` file to authenticate with the Kaggle API.
3.  Run the cells in the notebook sequentially. The notebook will automatically download the dataset, perform the EDA, and then train and evaluate each of the three models.
4.  The trained models and submission files will be saved to the `/content/` directory.

## Notebook Structure

The notebook is organized into the following sections:

1.  **Load Dataset**: This section handles the setup for downloading the glioma dataset from Kaggle.
2.  **Exploratory Data Analysis (EDA)**: A detailed analysis of the training data with visualizations.
3.  **ConvNeXtSmall Code**: The implementation, training, and evaluation of the ConvNeXtSmall model.
4.  **EfficientNetV2B0**: The implementation, training, and evaluation of the EfficientNetV2B0 model.
5.  **ResNet101V2**: The implementation, training, and evaluation of the ResNet101V2 model.
6.  **DenseNet201**: The implementation, training, and evaluation of the DenseNet201 model.
7.  **ViT-B/16**: The implementation, training, and evaluation of the Vision Transformer (ViT-B/16) model.

## Models

The notebook implements the following three deep learning models:

* **ConvNeXtSmall**: A modern CNN architecture that is designed to be simple and effective.
* **EfficientNetV2B0**: An efficient and scalable CNN that achieves high accuracy with fewer parameters.
* **ResNet101V2**: A deep residual network that is known for its strong performance in various computer vision tasks.
* **DenseNet201**: A convolutional neural network with dense connections between layers, which encourages feature reuse and strengthens feature propagation.
* **ViT-B/16**: A Vision Transformer model that applies the transformer architecture, originally from natural language processing, to image classification tasks.

Each model is fine-tuned on the glioma dataset, and its performance is evaluated on a validation set.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
