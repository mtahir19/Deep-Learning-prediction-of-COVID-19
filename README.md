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

## Objectives:
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

A **data science workflow** was implemented to conduct this analysis. Firstly, the **problem statement** was defined—the physicians needed to determine how to increase accuracy rates and improve COVID-19 control. Next, **data ** was downloaded by locating credible sources that housed the appropriate datasets: Images data scores and NLP predictions. Before beginning any analysis of the data, each individual dataset was imported to a **Pandas DataFrame**. Next, **data cleaning** was conducted to ensure that all datatypes were accurate and any other errors were fixed. Using all data, an **exploratory data analysis** was conducted to determine any parameters. Since the image datasets contain data from a random source, the parameters were measured, not sample statistics. Grid Search findings were used to then perform **data visualization and model predictions**. The following data visualizations were used to display the data: 
- Model-1: Convolutional Neural Network (CNN) and Early Stopping
- Model-2: Dropout Regularization
- Model-3: Regularization Method: L1 and L2

Once all data was visualized and all predictions are made.  To confirm and support the observations made, **external research** about the COVID-19 work and any other relevant data was conducted. Finally, well-informed **data-driven recommendations** for the physicians were compiled. 

**SIGNIFICANT FINDINGS**

When analyzing the datasets, few findings about SAT test scores and participation rates were gathered. Here are the most significant findings, focusing primarily on the SAT: 
- SAT Total Scores, 2017-18: The distribution of average test scores from all states was bimodal. Students either performed very poorly or very well. 
- SAT Participation Rates, 2017-18: The distribution of participation rates from all states appeared to be right skewed and slightly bimodal, where a majority of states experienced low participation rates, and only some had high participation rates. 
- SAT Test Scores vs Participation Rates, 2017-18: In both years, there was a strong negative correlation between test scores and participation rates. The higher the participation rate, the lower the test score. A concentration of states on the East Coast tended have a combination of high participation and low test scores. 

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
- Model Interpretability

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
According to a very recent scientific review-paper published in the "journal Nature Machine Intelligence" has identified a lot important findings. This search identified 2,212 studies, of which 415 were included after initial screening and, after quality screening, "only 62 studies were included in the systematic review". None of the 62 models was of potential clinical use, which is a major weakness, given the urgency with which validated COVID-19 models are needed.
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
I found that the College Board is focusing on increasing participation rates while not focusing on the outcome of test scores. There is a significant negative correlation between participation rates and test scores, which means that the higher the participation rates, the lower the test scores (and vice versa). Focusing solely on increasing participation rates by the College Board is equivalent to the College Board assisting in  deterioration of test scores. This may help in achieving an ideal of a 100% participation rate, however, a majority of US high schoolers will perform very poorly on the test.
<br>
**Outlook**
<br>
Therefore in order to achieve sustainable growth and be a resource trusted by students nationwide (i.e., its primary customers), I recommend the following:  
- Instead of keeping focus only on the participation rate, they must have to focus seriously towards improving access to test preparation resources. 
- Create a better test preparation support for states with highest participation rates, particularly in the East Coast where there is a concentration of states with high performance and low test scores.

--- 
## Data Sources
The sources of the datasets used in this analysis:

1 - https://scitechdaily.com/300-covid-19-machine-learning-models-have-been-developed-none-is-suitable-for-detecting-or-diagnosing/

2- https://www.nature.com/articles/s42256-021-00307-0

3 - http://www.aylward.org/notes/open-access-medical-image-repositories

4 - https://www.kaggle.com/search?q=lungs+image+segmentation+datasetFileTypes%3Ajpg+datasetSize%3Alarge

5- https://github.com/ieee8023/covid-chestxray-dataset
