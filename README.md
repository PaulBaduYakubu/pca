# pca
🔹 GitHub Short Description (for repository header)

Principal Component Analysis (PCA) on the Lycos-IDS2017 dataset for dimensionality reduction and visualization to enhance DDoS detection accuracy and interpretability.

🧠 Lycos-IDS2017 PCA Analysis
Feature Reduction and Visualization for DDoS Detection

📘 Abstract

This repository implements Principal Component Analysis (PCA) on the Lycos-IDS2017 dataset for dimensionality reduction and visualization in the context of Distributed Denial of Service (DDoS) attack detection.
The analysis identifies key features contributing to network anomalies, reduces data complexity, and supports downstream machine learning pipelines aimed at real-time intrusion detection.

🎯 Objectives

Apply PCA to reduce dataset dimensionality while preserving variance.

Identify and visualize correlations among original features.

Evaluate explained variance ratios to determine optimal component count.

Prepare transformed data for use in automated ML (TPOT) and interpretability (SHAP) experiments.

📂 Repository Structure
├── lycos_pca.ipynb           # Main PCA analysis notebook
├── requirements.txt          # Project dependencies
├── README.md                 # Documentation
└── data/
    └── Lycos-IDS2017.csv     # Dataset file (user-provided)

⚙️ Installation

Clone the repository and install dependencies:

git clone https://github.com/<your-username>/lycos-pca.git
cd lycos-pca
pip install -r requirements.txt

🧩 Requirements
# requirements.txt
pandas
numpy
matplotlib
seaborn
scikit-learn
joblib


✅ Tested with Python 3.9 and above.

💾 Dataset

Lycos-IDS2017 Dataset
A benchmark intrusion detection dataset for evaluating models against DDoS and other cyber attacks.
Obtain the dataset from the official Lycos-IDS2017 repository or your institutional data archive.

Citation:
Lycos-IDS2017 Dataset, Network Security Research Group, 2017.

Place the file in:

/data/Lycos-IDS2017.csv

🚀 Usage

Launch Jupyter Notebook:

jupyter notebook lycos_pca.ipynb


Run all cells sequentially to perform:

Data loading and preprocessing

Correlation heatmap analysis

PCA computation and visualization

Export of transformed feature space

📊 Key Results

Dimensionality reduced while preserving >95% total variance.

Identified feature redundancies and clusters using heatmaps.

Visualized top principal components to interpret dataset structure.

Generated PCA-transformed dataset for use in DDoS classification tasks.

🔍 Visualization Highlights

Correlation Matrix Heatmap – Detects redundant features.

Explained Variance Plot – Shows information retained per component.

2D PCA Projection – Visualizes normal vs attack traffic clusters.

🧠 Research Context

This analysis supports ongoing research on AI-driven DDoS detection systems.
The PCA-transformed dataset feeds into subsequent experiments using TPOT for automated model selection and SHAP for feature interpretability, forming part of the paper:

“Automated DDoS Detection Using TPOT and SHAP for Model Selection and Interpretability: A Study on Lycos-IDS2017 Dataset.”

📈 Future Work

Integrate PCA outputs into end-to-end automated ML pipelines.

Benchmark classifiers (e.g., Random Forest, XGBoost, SVM) on reduced features.

Conduct interpretability analysis using SHAP values.

👨‍💻 Author

Paul Badu Yakubu
Research Assistant, Fordham University
