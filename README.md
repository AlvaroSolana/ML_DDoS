# Machine Learning for DDoS Repository

## Overview

This repository contains Jupyter notebooks covering a machine learning pipeline designed to detect and characterize DDoS attacks. We applied both supervised and unsupervised learning techniques to analyze real network traffic flow and identify DDOS attacks flows

## Files

- **Section1\_Data\_exploration.ipynb**: Focuses on data preprocessing, visualization, and exploratory data analysis. The dataset has 85 features and 12 types of network traffic, including 11 different DDoS attack types. Techniques such as dimensionality reduction (PCA) and feature selection were applied.
- **Section2\_Supervised.ipynb**: Covers supervised learning methods like Random Forest, Logistic Regression, and K-Nearest Neighbors (KNN) for classifying network traffic. Hyperparameter tuning and cross-validation were used to achieve high classification accuracy (over 99%).
- **Section3\_Clustering.ipynb**: Implements unsupervised learning techniques, including K-Means and Gaussian Mixture Models (GMM), to identify hidden patterns in network traffic.

## Datasets Used

The following CSV files, contained in the `datasets.zip`, were used in this project:
- `ddos_dataset.csv` – Contains raw network traffic data, including 85 features and multiple types of DDoS attacks.
- `pca_training.csv` & `pca_testing.csv` – Created by performing Principal Component Analysis (PCA) on the original dataset. Used for supervised learning
- `df_processed.csv` – Created by eliminating highly correlated features to improve clustering performance. Used for unsupervised learning.

## Requirements

To run the notebooks, ensure you have the following dependencies installed:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/AlvaroSolana/ML_DDoS
   ```
2. Navigate to the project directory:
   ```bash
   cd ML_DDoS
   ```
3. Launch Jupyter Notebook:
   ```bash
   jupyter lab
   ```
   If you need to install jupyter lab: https://jupyter.org/install
   
5. Open and run the notebooks as needed.

## License

This project is open-source and available under the MIT License.

## Contact

For any questions or contributions, feel free to open an issue or reach out!

