# Latent SHAP for Counterfactual Explanations

## 📌 Project Overview

This project explores **Latent SHAP**, an extension of SHAP for non-interpretable feature spaces. We generate counterfactual explanations for deep learning models.

## 📂 Folder Structure

Latent-SHAP/
│── models/                    		# Store trained models (VAE, Classifier, Feature Extractor)
│── data/                   			# Dataset and extracted features
│   ├── train/              				# Training images
│   ├── test/               				# Test images
│   ├── latents/            				# Extracted latent vectors
│   ├── interpretable/      			# Extracted interpretable features
│── scripts/                			# Python scripts for each step
│   ├── extract_latents.py  			# Extract latent features from images
│   ├── extract_features.py 			# Extract interpretable features
│   ├── train_models.py     			# Train feature extractor CNN
│   ├── run_shap.py         			# Apply Latent SHAP
│   ├── generate_cf.py      			# Generate counterfactuals
│   ├── evaluate.py         			# Evaluate counterfactual explanations
│── results/                			# Store results
│   ├── original_images/    			# Original test images
│   ├── counterfactual_images/ 		# Generated counterfactuals
│   ├── shap_results.json   			# SHAP attributions
│   ├── evaluation_metrics.csv 		# SSIM, PSNR, UQI scores
│── notebooks/              		# Jupyter Notebooks for testing/debugging
│── requirements.txt        		# Minimal dependencies
│── .gitignore              			# Ignore unnecessary files
│── README.md               		# Documentation

## 🚀 Installation & Setup

1. **Create a virtual environment (Python 3.11+)**:
   ```bash
   python3.11 -m venv venv-shap
   source venv-shap/bin/activate
   ```
