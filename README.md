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
The main goal of the project was to stablize bike demand at every hour. Based on the objective, it was found that:
The Random Forest model achieved an R-squared value of 0.82 on both the training and test sets, indicating that the model generalizes well and captures a significant portion of the variance in the target variable.

  Bike rental count is high during working days than on weekend.

  Bike demand shows peek around 8-9 AM in the morning and 6 - 7pm in the evening.

  People prefer to rent bike more in summer than in winter.
