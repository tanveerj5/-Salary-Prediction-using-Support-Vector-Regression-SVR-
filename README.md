# 💰 Salary Prediction using Support Vector Regression (SVR)

This project implements **Support Vector Regression (SVR)** to predict salaries based on position levels using the `Position_Salaries.csv` dataset. 🚀

## 📌 Table of Contents
- [📖 Introduction](#introduction)
- [📊 Dataset](#dataset)
- [⚙️ Project Setup](#project-setup)
- [📏 Feature Scaling](#feature-scaling)
- [🧠 Training the SVR Model](#training-the-svr-model)
- [🔍 Making Predictions](#making-predictions)
- [📈 Visualizing the Results](#visualizing-the-results)
- [🔬 High-Resolution Visualization](#high-resolution-visualization)
- [🏁 Conclusion](#conclusion)

## 📖 Introduction
**Support Vector Regression (SVR)** is a powerful machine learning technique that uses **kernel functions** to map input data into higher-dimensional spaces, allowing for more accurate predictions. In this project, we apply **SVR with the Radial Basis Function (RBF) kernel** to predict salaries based on an employee's position level.

## 📊 Dataset
The dataset `Position_Salaries.csv` contains the following columns:
- **🏢 Position**: The job position (not used in the model)
- **📊 Level**: The numerical representation of the job position
- **💵 Salary**: The actual salary for that level

## ⚙️ Project Setup
The project involves **loading the dataset, extracting relevant features, and preparing the target variable** for regression analysis. **SVR** is used to model the relationship between the position level and salary.

## 📏 Feature Scaling
Feature scaling is **crucial** in SVR because the algorithm does not inherently normalize data like some other models. Since the **salary and position levels have different numerical ranges**, standardization ensures that both features contribute **equally** to the model’s training process. 

🔹 Without feature scaling, the model might be **biased towards features with larger numerical values**, leading to incorrect predictions.

## 🧠 Training the SVR Model
The **SVR model** is trained using a **Radial Basis Function (RBF) kernel**. 

🔹 **Why use a kernel?** 
The kernel trick enables SVR to **operate in a higher-dimensional feature space without explicitly transforming the input data**. This approach helps the model **capture complex nonlinear relationships** in the dataset, making it a great choice for this problem.

## 🔍 Making Predictions
To make predictions, the model **transforms new data using the same scaling method** applied during training. The **predicted salary is then inverse-transformed** to retrieve the actual scale of salary values.

## 📈 Visualizing the Results
The results are **visualized using Matplotlib** by plotting:
- The **original salary data points** (red dots) 🟥
- The **SVR prediction curve** (blue line) 🔵

This helps to assess how well the model fits the data.

## 🔬 High-Resolution Visualization
A **higher-resolution grid** is used to create a **smoother prediction curve**. This provides a more **detailed view of how SVR models the salary trend** across different position levels.

## 🏁 Conclusion
This project demonstrates how **SVR** can be used to predict salaries based on position levels, emphasizing:
✅ The **importance of feature scaling** 📏
✅ The **use of kernel-based regression techniques** 🧠
✅ The **visualization of results for better interpretation** 📈

The results are visualized using **Matplotlib** to show both **standard and high-resolution plots**. 🛠️✨

