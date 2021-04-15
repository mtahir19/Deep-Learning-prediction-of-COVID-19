# Deep Learning prediction of COVID-19 radiological imaging for improving the accuracy of diagnosis

- [Problem Statement](#Problem-Statement)
 - [Executive Summary](#Executive-Summary)
 - [prediction.ipynb contents](#prediction.ipynb-contents)
 - [interpretation.ipynb contents](#prediction.ipynb-contents)
 - [nlp.ipynb contents](#nlp.ipynb-contents)
 - [External Research](#External-Research)
 - [Conclusions & Outlook](#Conclusions-&-Outlook)
 - [Data Sources](#Data-Sources)

## Problem Statement:
A recent scientific review-paper published in Nature has found that out of the more than 300 COVID-19 machine learning models described in 2020 <sup>1</sup>. None of them is suitable for detecting or diagnosing COVID-19 from standard medical imaging. This is due to biases, methodological flaws, lack of reproducibility, and "Frankenstein" datasets.
The ability to predict the progress of the COVID-19 disease is crucial to decision making aimed at controlling the spread. There is no significant collection of COVID-19 chest X-rays or CT scans designed to be used for computational analysis.
In order to achieve success at large scale, questions to explore in such a situation are: Can we accurately classify and predict covid-19 through x-ray images or can we incorporate heterogeneous data sources (NLP) to improve the diagnostic ?

### Objectives:
To forecast the number of infections due to covid-19 with a maximum prediction accuracy (precision and recall : False negative is critical).

This would help physicians to make a fast decision with confidence by having a digital second opinion confirm their assessment of a patient's condition. Further, this can provide quantitative scores to consider and use in studies.

Image data linked with clinically relevant attributes in a public dataset that is designed for Machine Learning will enable parallel development of these tools and rapid local validation of models. Furthermore, this data can also be used for completely different tasks.

**Citations**:
<br>
<sup>1</sup> https://www.nature.com/articles/s42256-021-00307-0

---

## Executive Summary
**INTRODUCTION**

An analysis is conducted on the x-ray image for diaginisis of COVID-19. 931 images are taken to test different models. Analyzing scores and image data, the IEEE make their images and updated data available to the public. 

**METHODOLOGY**

A **data science workflow** was implemented to conduct this analysis. Firstly, the **problem statement** was defined—the physicians needed to determine how to increase accuracy rates and improve COVID-19 spread control. Next, **data ** was downloaded by locating credible sources that housed the appropriate datasets: Images data sets. Before beginning any analysis of the data, each individual dataset was imported to a **Pandas DataFrame**. Next, **data cleaning** was conducted to ensure that all data types were accurate and any other errors were fixed. Using all data, an **exploratory data analysis** was conducted to determine any parameters. Since the image datasets contain data from a random source, the parameters were measured, not sample statistics. Grid Search findings were used to then perform **data visualization and model predictions**. The following data visualizations were used to display the data: 
- Model-1: Convolutional Neural Network (CNN) and Early Stopping
- Model-2: Dropout Regularization
- Model-3: Regularization Method: L1 and L2
- Model Interpretability using SHAP
- Supported by Natural Language Processing model prediction

Once all data is visualized and some predictions are made.  To confirm and support the observations made, **external research** about the COVID-19 work and any other relevant data was conducted. Finally, well-informed **data-driven recommendations** for the physicians were compiled. 

**SIGNIFICANT FINDINGS**

When analyzing the datasets, few findings about COVID-19 images scores were gathered. Here are the most significant findings, focusing primarily on the images datasets: 
- Convolutional Neural Network (CNN) and Early Stopping: loss: 0.5565 - accuracy: 0.7130 - auc_1: 0.7819 - val_loss: 0.5665

-                 precision    recall  f1-score   support
-
 -          0       0.79      0.58      0.67        45
  -         1       0.74      0.89      0.81        62
-
 -   accuracy                           0.76       107
  - macro avg       0.77      0.73      0.74       107
- weighted avg       0.76      0.76      0.75       107

- Dropout Regularization: loss: 0.6714 - acc: 0.5908 - auc_2: 0.5993 - val_loss: 0.6714
 

- Regularization Method: L1 and L2: loss: 0.6580 - acc: 0.6382 - auc_3: 0.6827 - val_loss: 0.6587

- Indeed the score is best for the first simple NN model.


## Main Contents:
### prediction.ipynb Contents:
- Libraries and Data Import
- Exploratory Data Analysis
- Model-1: Convolutional Neural Network (CNN) and Early Stopping
- Model-2: Dropout Regularization
- Model-3: Regularization Method: L1 and L2

### interpretation.ipynb Contents:
- Libraries Imports and Data Reading
- Exploratory Data Analysis
- Model Training: Convolutional Neural Network (CNN)
- Model Interpretability using shap

### nlp.ipynb Contents:
- Libraries Import and Reading the Data
- Understanding some useful features
- Train-Test split and Base Line Model
- Natural Language Processing model prediction

- External Research
- Conclusions and Outlook

---

---
## External Research
According to a very recent scientific review-paper published in the "journal Nature Machine Intelligence" has identified a lot of important findings. This search identified 2,212 studies, of which 415 were included after initial screening and, after quality screening, "only 62 studies were included in the systematic review". None of the 62 models was of potential clinical use, which is a major weakness, given the urgency with which validated COVID-19 models are needed.
We believe that Machine Learning is a promising and potentially powerful technique for detection and prognosis of COVID-19 disease. Machine Learning models could enable a personalized approach to medicine through improved diagnosis and prediction of individual responses to therapies.

Some of the studies were hampered by issues with poor quality data, poor application of machine learning methodology, poor reproducibility, and biases in study design. A lot of the machine learning models were trained on sample datasets that were too small to be effective. Many other papers, the studies did not specify where their data had come from, or the models were trained and tested on the same data, or they were based on publicly available ‘Frankenstein datasets’ that had evolved and merged over time, making it impossible to reproduce the initial results. Therefore, in addition to higher quality datasets, manuscripts with sufficient documentation to be reproducible and external validation are required to increase the likelihood of models being taken forward and integrated into future clinical trials to establish independent technical and clinical validation as well as cost-effectiveness.

Citations
<br>
1: https://www.nature.com/articles/s42256-021-00307-0
<br>
2: https://scitechdaily.com/300-covid-19-machine-learning-models-have-been-developed-none-is-suitable-for-detecting-or-diagnosing/
<br>
3: http://www.aylward.org/notes/open-access-medical-image-repositories

---
## Conclusions & Outlook 
I found that the physicians are focusing on increasing x-ray image rates while not focusing on the quality of the images. There is a significant impact on processing and prediction rates of images, which means that the lower scores are related to not clean quality of the images taken. Secondly, we have to use the best possible models and good quality data, advanced application of machine learning methodology, good reproducibility, and biases in study design.
<br>
**Outlook**
<br>
Therefore, to achieve best score and highly improved predictions, I recommend the following:  
- we have to use large datasets 
- care should be taken with publicly available ‘Frankenstein datasets’.
- Need Sufficient documentation to be reproducible
- External validation are required to increase the likelihood of models

--- 
## Data Sources
The sources of the datasets used in this analysis:

1 - https://github.com/ieee8023/covid-chestxray-dataset

2 - http://www.aylward.org/notes/open-access-medical-image-repositories

3 - https://www.kaggle.com/search?q=lungs+image+segmentation+datasetFileTypes%3Ajpg+datasetSize%3Alarge