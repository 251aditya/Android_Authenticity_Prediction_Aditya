# [Android_Aunthenticity Prediction ](https://drive.google.com/file/d/1MdmsaoWiqf0wbCi7ct5knthob7fUDwfM/view?usp=sharing)
## Table of Contents
- [Introduction](#introduction)
- [Problem Statement](#problem_statement)
- [Dataset](#dataset)
- [Installation](#installation)
- [Conclusion](#conclusion)



## Introduction
Dataset Description:
This comprehensive dataset comprises over 30,000 Android applications sourced from diverse origins: Google Play Store, third-party app markets (hiapk, app china, Android, mumayi, gfan, slideme, pandaapp), and dedicated malware repositories.

Data Collection & Features:
Data Collection: Applications were meticulously collected over a three-year period, ensuring a continuous stream of data.
Feature Extraction: Key features extracted for each app encompass permissions requested during both installation and runtime. This granular approach provides a robust foundation for analysis.

Malware Representation:
Malware Families: The dataset encompasses 81 distinct malware families, offering a diverse and challenging landscape for malware detection models.
Binary Classification: The primary objective is to classify each app into one of two categories:
Benign (0): Applications with no malicious intent.
Malware (1): Applications exhibiting malicious behavior.

Data Format:
Feature File: A dedicated file outlines the complete list of extracted features.
.apk Files: Individual .apk files are associated with each app, containing detailed information about requested permissions and their respective packages.

Project Goals:
This dataset presents a valuable resource for developing and evaluating machine learning models capable of accurately detecting Android malware based on its permission usage patterns.

Potential Research Areas:
Malware Classification: Develop and fine-tune machine learning models (e.g., decision trees, random forests, neural networks) to effectively classify apps as benign or malicious.
Feature Importance Analysis: Investigate the significance of different permission groups in malware detection.

## Problem_Statement
The rapid growth of Android applications has led to a significant increase in the risk of malicious apps infiltrating the ecosystem. These malicious apps pose a serious threat to user privacy and security by stealing sensitive data, performing unauthorized actions, and potentially damaging devices. To mitigate this risk, it is imperative to develop a robust machine learning model capable of accurately predicting the authenticity of Android apps.

So we can understand Android application (app) is authentic or not. With the increase in the number of mobile apps, the risk of downloading malicious apps has also increased. Malicious apps can steal sensitive user data, perform unwanted actions, and damage the user's device. Therefore, it is essential to develop a model that can accurately predict the authenticity of Android apps and help users make informed decisions about which apps to download and install on their devices. The challenge is to identify the relevant features that can distinguish between authentic and malicious apps and to train a classification model that can generalize well to new, unseen apps. Additionally, the model should be able to handle the large and dynamic nature of the mobile app ecosystem, where new apps are constantly being developed and released.

Ultimately, the success of this project will contribute to a safer and more secure Android ecosystem, empowering users to navigate the vast app marketplace with confidence.

## Dataset
The dataset used in this project is sourced from [here](https://drive.google.com/file/d/1MdmsaoWiqf0wbCi7ct5knthob7fUDwfM/view?usp=sharing) It comprises a comprehensive collection of information related to Android Authenticity Prediction, including:

Input Columns (184 variables) and Rows(30000).

## Installation
To run this project on your local machine, follow these steps:

         Copy the colab file into your drive.

         Run the colab file to gain insights.

## Conclusion
In this project, we focused on detecting malicious Android applications using various machine learning classification techniques. After evaluating multiple models including Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, and XGBoost Classifier, we chose the **XGBoost Classifier** as our final model.

🔍 **Model Evaluation & Selection**
![Alt text](path/to/your/model.png)


While Logistic Regression showed slightly higher performance in terms of accuracy and ROC AUC after cross-validation, **XGBoost was selected as the final model** due to several key advantages:

  * Robustness to non-linearity and feature interactions

  * Built-in regularization, reducing the risk of overfitting

  * Strong handling of imbalanced datasets

  * Explainability through SHAP values and feature importance plots

🔐 **Security Insight: The Role of Permissions**
App permissions play a vital role in distinguishing between safe and malicious apps. In our feature engineering, permissions like **Device Admin, SMS & Calls, Camera, and Location** were strongly associated with malware. In contrast, permissions such as **Internet Access, WiFi State, and Vibration Control** were more commonly requested by benign applications.

🤖 **AI-Powered Malware Detection**
Our classifier serves as an **AI-based malware authenticator** that can be integrated into existing security frameworks. This model, when deployed:

  * Provides real-time threat detection

  * Enhances mobile security

  * Assists users and app store platforms in identifying risky apps before installation

✅ **Final Takeaway**
The **XGBoost Classifier** offered the best trade-off between performance and practical robustness. Combined with feature-level insights and high scalability, the Android Authenticity Prediction model is a powerful tool in the fight against evolving mobile threats. Continued refinement of this model will help stay ahead of increasingly sophisticated malware.
