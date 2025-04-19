# Digit Recognizer

This project implements a digit recognition system using the K-Nearest Neighbors (KNN) algorithm. It includes preprocessing, dimensionality reduction using Principal Component Analysis (PCA), and model evaluation.

---



## Features

- **Dataset Loading**: Reads the digit dataset from a CSV file.
- **Visualization**: Displays sample images from the dataset.
- **Dimensionality Reduction**: Uses PCA to reduce the feature space for faster computation.
- **Model Training**: Implements KNN with and without PCA.
- **Performance Evaluation**: Measures accuracy and execution time for different PCA components.
- **Pipeline Creation**: Combines PCA and KNN into a single pipeline for streamlined processing.
- **Model Export**: Saves the trained model as a `.pkl` file for future use.

## Usage Guide: Digit Recognizer with KNN and PCA

#### 1. Load the Dataset
- The dataset is loaded from `digit-recognizer_train.csv`.

#### 2. Visualize Data
- View sample images and their corresponding labels to understand the dataset.

#### 3. Train-Test Split
- Split the dataset into **training** and **testing** sets for model evaluation.

#### 4. Run KNN Without PCA
- Train and evaluate the **K-Nearest Neighbors (KNN)** model on the full feature set.

#### 5. Run KNN With PCA
- Apply **Principal Component Analysis (PCA)** to reduce the number of features.
- Train and evaluate the **KNN** model on the reduced feature set.

#### 6. Find Optimal PCA Components
- Evaluate the model’s **accuracy** and **execution time** across different numbers of PCA components to select the optimal configuration.

#### 7. Create a Pipeline
- Combine **PCA** and **KNN** into a single pipeline for streamlined training and testing.

#### 8. Export the Model
- Save the trained pipeline as `digit_recognizer.pkl` for future use.

----

## Results

#### KNN Without PCA
- **Accuracy**: 96.6%
- **Execution Time**: 7.12seconds

#### KNN With PCA
- **Accuracy**: 96.5% (with 250 components)
- **Execution Time**: 4.7 seconds

#### Optimal PCA Components
- **Best Number of Components**: 51
- **Accuracy**: 97.3%
- **Execution Time**: 0.52 seconds

#### Pipeline Performance
- **Accuracy**: 97.3% (with 51 components)


### Exported Model
- The trained pipeline is saved as `digit_recognizer.pkl` and can be reused for predictions without retraining.