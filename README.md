# Insight-A_Cut_Above

### A Cut Above: Finding the Sharpest Surgeon

The Jupyter Notebook in this repository contains the code used to build a model that classifies lung surgeons based on their predicted rate of negative surgical outcomes. The model was constructed using data scraped from several public websites and the class designations that it output were incorporated into a [web app](https://cut-above.herokuapp.com) that allows users to search for lung surgeons in their local area.

#### Data

The following data was scraped and combined:

1. Physician-level surgical outcome and demographic data from Checkbook.org
2. Hospital ratings for lung surgery and pulmonology from U.S. News and World Reports
3. Ratings information from patient review websites such as Healthgrades.com

#### Model

Surgeon quality was predicted using ground truth surgical outcome data to classify each surgeon into one of three groups. A gradient boosting classifier was trained following upsampling using SMOTE. In spite of the high bias of the dataset, the model was able to successfully assign surgeons to their proper class more frequently than with random assignment. Further, surgeons assigned to the highest class had a significantly lower rate of negative outcomes than the average surgeon in the dataset.
