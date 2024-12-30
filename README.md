# Loan Applicant Risk Segmentation

## Overview

This project focuses on analyzing and classifying loan applicants based on various features such as **Age**, **Total Work Experience**, **Number of Years in City**, **Cost to Request Ratio**, **Cibil Score**, **Overdrafts (Past 12 Months)**, and **Total Bounces (Past 12 Months)**. The objective is to predict and segment the risk of loan applicants, specifically focusing on the **Total Bounces in the past 12 months** as the target variable. The project is divided into two phases: data exploration and model building.

---

## Dataset

The dataset contains the following columns:
- **Age**: Age of the applicant.
- **Total Work Experience**: Total work experience in years.
- **Number of Years in City**: Duration of time the applicant has lived in the current city.
- **Cost to Request Ratio**: Ratio of the requested loan amount to the applicant's income.
- **Cibil Score**: Applicant's credit score.
- **Overdrafts (Past 12 Months)**: Number of overdrafts in the past year.
- **Total Bounces (Past 12 Months)**: Target variable indicating the total number of bounces (defaults or missed payments) in the past year.

---

## Project Phases

### Phase 1: Data Exploration and Preprocessing

In this phase, the dataset is loaded and preprocessed:
- The dataset is inspected for any **null values** and basic information is extracted.
- Basic statistical details are generated using the `describe()` function.
- Visualizations are created, including a **scatter plot** between **Age** and **Total Work Experience**, and **box plots** for **Age** and **Cibil Score**.
- The target variable (**Total Bounces Past 12 Months**) and features are separated.

### Phase 2: Model Building

In this phase, the model is created and evaluated:
- The data is split into **training** and **testing** sets.
- A **K-Nearest Neighbors (KNN)** classifier is used to model the relationship between the features and the target variable.
- The model's performance is evaluated by displaying the **training score**, **testing score**, and **accuracy score**.
- The classifier is tested with **k-values** ranging from 1 to 14 to find the optimal value for the best model performance.
