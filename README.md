# ESP-Fi HAR: WiFi Human Activity Recognition

## Project Overview

This project focuses on Human Activity Recognition (HAR) using WiFi Channel State Information (CSI). It explores how WiFi signals can be used to recognize different human activities without relying on wearable sensors.

The project investigates whether combining CSI amplitude information with phase-derived features can improve activity recognition, particularly when evaluating the model on subjects it has not seen during training.

## Objectives

- Recognize human activities using WiFi CSI data.
- Develop a lightweight dual-stream 1D CNN model.
- Compare model performance using different input features.
- Evaluate generalization to unseen subjects using Leave-One-Subject-Out (LOSO) validation.

## Activities

The dataset includes seven human activities:

- Running
- Falling
- Walking
- Turning
- Jumping
- Squatting
- Waving an arm

## Dataset

This project uses the **ESP-Fi HAR dataset**.

The data contains WiFi CSI measurements collected across different environments and participants.

Dataset source: [ESP-Fi HAR on GitHub](https://github.com/AutoSmartGroup/ESP-Fi-HAR)

Please refer to the original dataset repository for its license, usage conditions, and complete data description.

##  Model and Methodology

The project explores a dual-stream 1D Convolutional Neural Network (CNN) that uses:

- **Amplitude stream:** extracts features from CSI amplitude measurements.
- **Phase-derived stream:** uses phase-related features derived from the CSI I/Q measurements.
- **Feature fusion:** combines information from both streams for activity classification.
- **Subject-independent evaluation:** uses Leave-One-Subject-Out (LOSO) validation to evaluate performance on unseen participants.

##  Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- PyTorch
- SciPy

##  How to Run

1. Clone or download this repository.
2. Install Python and Jupyter Notebook.
3. Install the required Python libraries.
4. Download the ESP-Fi HAR dataset from the original dataset repository.
5. Update the dataset path in the notebook to match your computer.
6. Open esp_fi_har_notebook_fixed_memory.ipynb in Jupyter Notebook.
7. Run the notebook cells in order.

Install the commonly used libraries with:

bash
pip install numpy pandas matplotlib scikit-learn scipy torch jupyter

The notebook may require additional setup depending on your dataset directory structure and the code cells you run.

## Evaluation

The project evaluates human activity classification using subject-independent validation. Relevant metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

The results should be reported after running the experiments and confirming the final evaluation outputs.

**Repository Structure**

text
ESP-Fi-HAR/
├── esp_fi_har_notebook_fixed_memory.ipynb
└── README.md

The dataset and experiment outputs may be stored separately and added to the repository when appropriate.

## 👩‍💻 Author

Progga Fariba Haq



Thanks to the authors of the ESP-Fi HAR dataset for making the dataset available for research.

