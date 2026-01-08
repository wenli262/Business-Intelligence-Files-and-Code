# Business-Intelligence-Files-and-Code
This repository contains the cleaned dataset, preprocessing scripts, and machine learning code developed for a Business Intelligence (BI) predictive analytics project focused on inventory understock risk prediction.

Two predictive models were implemented and compared:
- Logistic Regression  
- Random Forest  


The objective of this project is to evaluate model performance and develop predictive models that support proactive inventory replenishment, reduced stock-outs, lower operational risk, and more sustainable inventory management, aligned with SDG 12: Responsible Consumption and Production.

---

## Dataset
The dataset used in this study represents SKU-level inventory, sales, and supplier information and has undergone systematic preprocessing to ensure data quality and modelling suitability.

**Key characteristics:**
- Final dataset size: **10,000+ SKU records (after cleaning)**
- Target variable: `Understock`
- Numerical features include:
  - Weeks_Inventory
  - Available_Stock
  - Quantity_On_Hand
  - Sales_Volume
  - Demand and inventory turnover indicators
    
- Categorical features include:
  - SKU_ID
  - Product_Category
  - Supplier
  - Sales_Channel

The cleaned dataset is included in this repository for reproducibility.

---

## Repository Structure
This repository includes the following scripts and notebooks:

- **Data Preprocessing**
  - Data cleaning and validation
  - Handling missing values
  - Feature engineering
  - Encoding categorical variables
  - Feature scaling for Logistic Regression

- **Model Implementations**
  -Logistic Regression (binary classification)
  - Random Forest (ensemble classification)

Each model includes Training and testing phases, Probability-based predictions, Confusion matrix and classification metrics, Feature importance analysis

---

## Google Colab Notebook
All preprocessing and model training steps can be executed directly using Google Colab:

**Google Colab Link:**  
[https://colab.research.google.com/drive/1ZtCrbmm1F4ycsc8-43XK3h4M-0U1mRk8?usp=sharing]

The notebook provides an end-to-end workflow, including data loading, preprocessing, model training, and performance evaluation.

---

## Evaluation Strategy
Model performance is evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
  
This evaluation approach ensures balanced assessment of both stock-out risk detection and false alert minimisation, which are critical for inventory decision-making.
---

## Key Findings
- EBoth models achieved very high predictive performance, indicating strong data quality and feature relevance.
- Random Forest achieved perfect classification on the test dataset, with no false positives or false negatives.
- Logistic Regression successfully identified all understock cases, but produced a small number of false positives.
- Inventory-related variables such as Weeks of Inventory and Available Stock were consistently the most influential predictors across both models.
- Logistic Regression offers higher interpretability, while Random Forest provides stronger predictive reliability.

---
## Business Intelligence Implications
- The results demonstrate how predictive analytics can be integrated into BI systems to:
- Identify high-risk SKUs before stock-outs occur
- Support data-driven replenishment planning
- Reduce emergency restocking and operational costs
- Minimise inventory waste
- Improve overall supply chain sustainability

---

## Usage
1.Clone this repository
2.Open the provided notebooks or scripts
3.Load the cleaned dataset
4.Execute preprocessing and model training steps
5.Review model outputs, metrics, and feature importance results  

---

## Data Source
Supply Chain Inventory Management  
(https://www.kaggle.com/datasets/mustofaahmad/inventory-management-grocery-industry/data?select=Inventory+Management+E-Grocery+-+InventoryData.csv)
