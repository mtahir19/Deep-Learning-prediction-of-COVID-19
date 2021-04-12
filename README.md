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

Objectives:
To forecast the number of infections due to covid-19 with a maximum prediction accuracy (precision and recall : False negative is critical)

## Expected outcomes:

Tool impact: This would give physicians an edge and allow them to act with more confidence while they wait for the analysis of a radiologist by having a digital second opinion confirm their assessment of a patient's condition. Also, these tools can provide quantitative scores to consider and use in studies.

Data impact: Image data linked with clinically relevant attributes in a public dataset that is designed for ML will enable parallel development of these tools and rapid local validation of models. Furthermore, this data can be used for completely different tasks.

**Citations**:
<br>
<sup>1</sup> https://www.nature.com/articles/s42256-021-00307-0

---

## Executive Summary
**INTRODUCTION**

An analysis is conducted on the x-ray image for giaginisis of COVID-19. Each dataset contains state-by-state average test scores and participation rates, specifically from 2017 and 2018. Analyzing test scores and participation rates, the SAT make their test scores and participation data available to the public. 

**METHODOLOGY**

A **data science workflow** was implemented to conduct this analysis. Firstly, the **problem statement** was defined—the College Board needed to determine how to increase participation rates of the SAT. Next, **data scraping** was performed by locating credible sources that housed the appropriate datasets: SAT test scores and participation rates from 2017-18. Before beginning any analysis of the data, each individual dataset was imported to a **Pandas DataFrame**. Next, **data cleaning** was conducted to ensure that all datatypes were accurate and any other errors were fixed. Using all data from both years, an **exploratory data analysis** was conducted to determine any parameters. Since the SAT datasets contain data from an entire population of high school students from the class of 2017 and 2018, the population parameters were measured, not sample statistics. All statistical findings were used to then perform **data visualization**. The following data visualizations were used to display the data: 
- heat map
- histograms
- boxplots 
- scatterplots

Once all data was visualized and all statistical summaries were conveyed, **descriptive and inferential statistical analysis** was conducted to describe what the distributions were and any trends appeared in the data.  To confirm and support the observations made, **external research** about the SAT and any other relevant data was conducted. Finally, well-informed **data-driven recommendations** for the College Board were compiled. 

**SIGNIFICANT FINDINGS**

When analyzing the datasets, few findings about SAT test scores and participation rates were gathered. Here are the most significant findings, focusing primarily on the SAT: 
- SAT Total Scores, 2017-18: The distribution of average test scores from all states was bimodal. Students either performed very poorly or very well. 
- SAT Participation Rates, 2017-18: The distribution of participation rates from all states appeared to be right skewed and slightly bimodal, where a majority of states experienced low participation rates, and only some had high participation rates. 
- SAT Test Scores vs Participation Rates, 2017-18: In both years, there was a strong negative correlation between test scores and participation rates. The higher the participation rate, the lower the test score. A concentration of states on the East Coast tended have a combination of high participation and low test scores. 

## Main Contents:
### prediction.ipynb Contents:
- Description of the chest X-ray images
- Data Import & Cleaning
- Exploratory Data Analysis
- Convolutional Neural Network (CNN) and Early Stopping
- Dropout Regularization
- Regularization Method: L1 and L2

### interpretation.ipynb Contents:
- Description of the chest X-ray images
- Data Import & Cleaning
- Exploratory Data Analysis
- Convolutional Neural Network (CNN) and Early Stopping
- Dropout Regularization
- Regularization Method: L1 and L2

### nlp.ipynb Contents:
- Description of the chest X-ray images
- Data Import & Cleaning
- Exploratory Data Analysis
- Convolutional Neural Network (CNN) and Early Stopping
- Dropout Regularization
- Regularization Method: L1 and L2

- External Research
- Conclusions and Outlook

---

---
## External Research
Around 2 million students from the class of 2018 took the SAT, the highest ever.$^{1}$ In fact, there was a 27% increase in participation rates from the previous year.$^{2}$ SAT participation rates are so high that as of 2018, the test holds the title for "most widely used college admission test," beating the ACT where 1.91 million students took that test in the same year.$^{3}$  Although the SAT can celebrate this achievement, the data shows that there is a negative correlation between participation rates and test scores. This means that the higher the participation rate amongst all states the lower the average student test scores. 

Contrary to the College Board's claim that the SAT offers "greater access and opportunity" for students who take their test. But the higher the chances are of more students performing poorly. If taking the SAT is a significant contributor to college acceptance, the SAT itself is posing a burden to students' access to college. Instead of focusing on increasing participation rates, the SAT shows focus more test preparation resources.  

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
