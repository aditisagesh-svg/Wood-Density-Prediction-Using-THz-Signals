# Internship Project: Wood Defect Detection and Density Prediction Using THz and X-ray Imaging

This repository contains the complete implementation of my internship project conducted at CSIR-CEERI. The project focused on the use of Terahertz (THz) time-domain signals and X-ray image data to develop machine learning models for:

- Detecting internal defects (holes) in wood samples
- Predicting the wood density of diverse and tropical wood species


## Results Summary

Task | Best Model | R² Score | MAE (kg/m³)
-----|------------|----------|-------------
THz-based Density Prediction | Stacked (RF + XGBoost + Ridge) | 0.9985 | 4.74
X-ray-based Density Prediction | Stacked (CatBoost + RF + XGBoost) | 0.9997 | 2.73
Defect Detection | Pixel-level STD + Random Forest | Visual Analysis | —

## Technologies and Tools Used

- Python, Google Colab
- Libraries: NumPy, Pandas, Matplotlib, scikit-learn, XGBoost, CatBoost
- Signal Analysis Techniques: FFT, STFT, STD
- Machine Learning: Feature Engineering, Leave-One-Species-Out Cross-Validation, Stacked Ensemble Modeling

## Dataset

The dataset includes 110 wood samples (78 diverse and 32 tropical) and contains:
- 4D THz signals with shape [T, H, W, F]
- X-ray grayscale images
- CSV metadata including wood mass, volume, moisture content, dimensions, and species labels

Source: "Non-Destructive Wood Analysis Dataset: Comparing X-Ray and Terahertz Imaging Techniques"

Note: Due to size constraints, the dataset is not uploaded to this repository. It can be shared via Google Drive upon request.


