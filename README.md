# ANN-Concrete-Strength-Prediction

## Project Overview
This project aims to predict the compressive strength of concrete based on its composition and age using Artificial Neural Networks (ANN). The dataset, provided by a cement and concrete research company, contains information on various concrete mixtures and their corresponding compressive strengths.

## Problem Statement
Given the composition of a concrete mixture (including cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, and fine aggregate) and its age, predict the concrete's compressive strength in megapascals (MPa).

## Dataset Description
The dataset includes the following features:

| **Column**                 | **Description**                    |
|----------------------------|------------------------------------|
| Cement                     | kg in a m³ mixture                 |
| Blast Furnace Slag         | kg in a m³ mixture                 |
| Fly Ash                    | kg in a m³ mixture                 |
| Water                      | kg in a m³ mixture                 |
| Superplasticizer           | kg in a m³ mixture                 |
| Coarse Aggregate           | kg in a m³ mixture                 |
| Fine Aggregate             | kg in a m³ mixture                 |
| Age                        | Day (range: 1 to 365 days)         |
| Concrete Compressive Strength | MPa (target variable)           |

## Project Scope
The scope of this project includes:

- **Exploratory Data Analysis (EDA):** Understanding the data distribution, identifying correlations, and handling outliers.
- **Data Preprocessing:** Feature scaling using standardization and splitting the data into training and test sets.
- **ANN Model Development:** Building and training three different ANN architectures.
- **Model Evaluation:** Assessing the performance of each model using the R² score.
- **Model Tuning:** Refining the models by adjusting the number of layers, experimenting with different activation functions, and adding a dropout layer.

## Steps Undertaken

1. **Data Exploration:**
   - Loaded the dataset and visualized distributions using the `dist_custom` function.
   - Created boxplots to identify outliers and examine the spread of the data.
   - Generated a correlation matrix to understand relationships between features.
   - Used `sns.pairplot(data=df, diag_kind="hist")` to visualize pairwise relationships and distributions.

2. **Data Preprocessing:**
   - Performed feature scaling using standardization.
   - Split the data into training and test sets.

3. **Model Development:**
   - Created three different ANN architectures:
     - **Model 1:** Initial simple architecture, which resulted in an R² score of -4.95.
     - **Model 2:** Improved architecture, achieving an R² score of 0.81.
     - **Model 3:** Final model, slightly optimized, resulting in an R² score of 0.80.

4. **Model Tuning:**
   - Experimented with different numbers of layers and activation functions.
   - Added a dropout layer in the final model to prevent overfitting.

## Conclusion
The project successfully demonstrates how ANN can be used to predict concrete compressive strength. While the second model provided the best results, further improvements could be achieved by fine-tuning hyperparameters or experimenting with more advanced architectures.



