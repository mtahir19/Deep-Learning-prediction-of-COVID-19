# Deep Learning prediction of COVID-19 radiological imaging for improving the accuracy of diagnosis
Problem statement: Can we accurately classify and predict diagnose covid-19 images: Also incorporate heterogeneous data source (NLP) to improve the diagnostic.

Background:
In the context of a COVID-19 pandemic, we want to improve prognostic predictions to triage and manage patient care. Data is the first step to developing any diagnostic/prognostic tool. While there exist large public datasets of more typical chest X-rays from the NIH [Wang 2017], Spain [Bustos 2019], Stanford [Irvin 2019], MIT [Johnson 2019] and Indiana University [Demner-Fushman 2016], there is no collection of COVID-19 chest X-rays or CT scans designed to be used for computational analysis.

Context/situation:
The ability to predict the progress of the disease is crucial to decision making aimed at controlling the spread

Objectives:
To forecast the number of infections due to covid-19 with a maximum prediction accuracy (precision and recall : False negative is critical)

## Models (potentially):
- CNN: classification to see if the patient has covid or not
- CNN: if patient has covid then explore damage regions in image data
- NLP: Using NLP to analyze text data to improve diagnosis.
- Transfer Learning
- SKlearn and tensorflow.keras
- Pytorch and compare with tensorflow.keras
## Expected outcomes:

Tool impact: This would give physicians an edge and allow them to act with more confidence while they wait for the analysis of a radiologist by having a digital second opinion confirm their assessment of a patient's condition. Also, these tools can provide quantitative scores to consider and use in studies.

Data impact: Image data linked with clinically relevant attributes in a public dataset that is designed for ML will enable parallel development of these tools and rapid local validation of models. Furthermore, this data can be used for completely different tasks.

## References:

1 - https://scitechdaily.com/300-covid-19-machine-learning-models-have-been-developed-none-is-suitable-for-detecting-or-diagnosing/

2- https://www.nature.com/articles/s42256-021-00307-0

3 - http://www.aylward.org/notes/open-access-medical-image-repositories

4 - https://www.kaggle.com/search?q=lungs+image+segmentation+datasetFileTypes%3Ajpg+datasetSize%3Alarge

5- https://github.com/ieee8023/covid-chestxray-dataset
