# BreastCancerClustering

## Description
This repository contains a Python implementation of K-Means clustering and Principal Component Analysis (PCA) applied to the Breast Cancer Wisconsin (Diagnostic) dataset. The project demonstrates data preprocessing, K-Means clustering from scratch, PCA for dimensionality reduction, and visualization of clustering results before and after PCA. The code evaluates clustering performance using metrics like Sum of Squared Errors (SSE) and Silhouette Score, and visualizes the results using the Elbow Method and PCA projections in 1D, 2D, 3D, and 4D.

## Repository Structure
- `BreastCancerClustering.ipynb`: The main Python script containing the implementation of K-Means clustering, PCA, and visualization.
- `requirements.txt`: Lists the required Python libraries to run the code.
- `README.md`: This file, providing an overview of the repository.

## Requirements
To run the code, you need Python 3.6+ and the following libraries:
- numpy
- pandas
- scikit-learn
- matplotlib

Install the dependencies using:
```bash
pip install -r requirements.txt
```

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/KarenSamehS/BreastCancerClustering.git
   ```
2. Navigate to the repository directory:
   ```bash
   cd BreastCancerClustering
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the main script:
   ```bash
   python BreastCancerClustering.ipynb
   ```

## Features
- **Data Preprocessing**: Loads and standardizes the Breast Cancer dataset using `StandardScaler`.
- **K-Means Clustering**: Custom implementation of the K-Means algorithm with configurable clusters, iterations, and tolerance.
- **PCA Implementation**: Custom PCA to reduce dimensionality and visualize data in 1D, 2D, 3D, and 4D.
- **Evaluation**: Computes Silhouette Score and SSE for clustering evaluation, and uses the Elbow Method to determine the optimal number of clusters.
- **Visualization**: Plots PCA results, Elbow Method curves, Silhouette Scores, and compares K-Means clustering before and after PCA.

## Output
Running `BreastCancerClustering.ipynb` will generate:
- Console output with Silhouette Scores and SSE values for different numbers of clusters.
- Plots showing:
  - Elbow Method for optimal cluster selection.
  - Silhouette Scores for clustering quality.
  - PCA visualizations in 1D, 2D, 3D, and 4D.
  - Comparison of K-Means clustering results before and after PCA.

## Key Observations
- PCA improves cluster separation by reducing noise and focusing on significant features.
- The optimal number of clusters is around \( k=2 \), aligning with the dataset's benign and malignant classes, though \( k=3 \) may reveal subgroups.
- Silhouette Scores and SSE indicate better clustering performance after PCA.
