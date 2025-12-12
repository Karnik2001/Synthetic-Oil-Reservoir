# Synthetic Oil Reservoir Using Machine Learning

## 📌 Project Overview

In traditional oil exploration, identifying promising reservoirs involves manual geological analysis, which can be slow and expensive. This project automates the prediction process by using supervised machine learning models on a synthetic dataset, offering a proof of concept that can be scaled to real-world data.

## 🎯 Objectives

- Predict whether a reservoir has high or low productivity based on its features.
- Evaluate multiple machine learning models to compare performance.
- Visualize model performance with confusion matrices and ROC curves.
- Explore the feasibility of using AI for reservoir classification in upstream energy.

## 🛠️ Technologies Used

- **Python 3.x**
- **Google Colab**
- **Pandas**, **NumPy** – Data manipulation
- **Matplotlib**, **Seaborn** – Visualization
- **Scikit-learn** – Machine learning algorithms and evaluation
- **XGBoost** – Advanced ensemble learning

## 🧾 Dataset Description

The dataset is synthetic but simulates realistic subsurface and geological properties relevant to oil reservoir identification. It includes the following features:

1️⃣ **Rock_Type** 🏔️  
   - The primary rock formation in the area:  
     - *Sandstone*, *Limestone*, or *Shale*  
   - Sandstone and Limestone are generally better reservoirs, while Shale is less favorable.

2️⃣ **Porosity (%)** 🌊  
   - Indicates how much empty space exists in the rock.  
   - Higher porosity means more room to store oil.  
   - Values range from **0% to 30%**.

3️⃣ **Permeability (mD)** 🛢️  
   - Measures how easily fluids can move through the rock.  
   - Higher permeability = better oil flow.  
   - Ranges from **1 to 1000 millidarcies (mD)**.

4️⃣ **Trap_Type** ⛏️  
   - Describes the geological trap structures:
     - *Anticline* (folded layers)  
     - *Fault* (displaced layers)  
     - *Dome* (circular uplift)  
     - *None* (no significant structure)  
   - Traps help oil accumulate and are crucial for reservoir formation.

5️⃣ **Seismic_Score** 🎵  
   - A score from **0 to 1** derived from seismic survey data.  
   - Higher scores indicate higher likelihood of finding oil.

6️⃣ **Proximity_to_Oil_Field (km)** 📍  
   - Distance to the nearest known oil field.  
   - Closer fields (0–5 km) suggest similar geological formations and higher success chances.

7️⃣ **Estimated_Reservoir_Depth (m)** 🔎  
   - Predicted depth of oil-bearing layers from **500m to 5000m**.  
   - Deeper layers may contain more oil but are harder to extract.

8️⃣ **Oil_Presence (Target)** ✅❌  
   - Binary classification target:
     - `1` = Oil Found  
     - `0` = No Oil

## 🧠 Methodology

1. **Data Cleaning** – Removal of null values and formatting.
2. **Feature Engineering** – Encoding categorical variables and scaling continuous features.
3. **Model Training** – Applied multiple classifiers:
   - Logistic Regression
   - Decision Tree
   - Random Forest
   - K-Nearest Neighbors
   - XGBoost
   - SVM
4. **Model Evaluation** – Compared performance using classification metrics.

## 📏 Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC-AUC Score**
- **Confusion Matrix**

## 📈 Results

✅ **Best Model: Logistic Regression**

- **Accuracy**: ~87%
- **Precision**: 0.85
- **Recall**: 0.89
- **F1 Score**: 0.87
- **AUC Score**: 0.91

A high AUC of 0.91 indicates excellent ability to distinguish productive vs. non-productive reservoirs, with low false positives and high recall.

## 📊 Visualization

- Confusion Matrices
- ROC Curves
- Feature Distributions
- Accuracy Comparison Across Models

Visual analysis complements metric evaluation to provide insights into prediction behavior and decision thresholds.

## Citations

https://www.geeksforgeeks.org/ml-logistic-regression-using-python/

https://www.datacamp.com/tutorial/decision-tree-classification-python

https://www.datacamp.com/tutorial/random-forests-classifier-python

https://www.datacamp.com/tutorial/xgboost-in-python

https://www.datacamp.com/tutorial/svm-classification-scikit-learn-python


