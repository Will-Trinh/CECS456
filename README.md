# 🐾 Animals-10 Image Classification

This project implements a Convolutional Neural Network (CNN) to classify images of animals into 10 categories using the **Animals-10** dataset sourced from Kaggle.

## 📂 Dataset
The dataset used is [Animals-10](https://www.kaggle.com/datasets/alessiocorrado99/animals10). It contains images for the following classes:
*   Cane (Dog)
*   Cavallo (Horse)
*   Elefante (Elephant)
*   Farfalla (Butterfly)
*   Gallina (Chicken)
*   Gatto (Cat)
*   Mucca (Cow)
*   Pecora (Sheep)
*   Ragno (Spider)
*   Scoiattolo (Squirrel)

## 🛠️ Prerequisites
*   Python 3.x
*   **Libraries**: `tensorflow`, `numpy`, `matplotlib`, `seaborn`, `kaggle`
*   **Kaggle API Token**: A `kaggle.json` file from your Kaggle account is required to download the dataset programmatically.

## 🚀 How to Run

1.  **Open the Notebook**:
    Load the `.ipynb` file in Google Colab or Jupyter Notebook.

2.  **Setup Kaggle API**:
    *   The first cell requires you to upload your `kaggle.json` API key.
    *   If running locally, place `kaggle.json` in `~/.kaggle/`.

3.  **Execute Cells**:
    Run the cells sequentially to:
    *   Download and unzip the dataset.
    *   Preprocess the images (resize to 128x128, normalize).
    *   Train the CNN model (default: 15 epochs).
    *   Visualize accuracy/loss plots and the confusion matrix.

## 🧠 Model Architecture
*   **Input**: (128, 128, 3) RGB images.
*   **Structure**: Three Convolutional blocks (Conv2D + MaxPooling), followed by a Flatten layer, a Dense hidden layer (128 units), Dropout (0.5), and a final Softmax Output layer.

## 📊 Results
The notebook outputs:
*   Training vs. Validation Accuracy/Loss curves.
*   A Confusion Matrix heatmap to visualize misclassifications.
*   A Classification Report with Precision, Recall, and F1-scores.
