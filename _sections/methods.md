---
title: "Methods"
order: 3
---

The present report applies PCA to activity monitoring data in order to build a model to predict subject age. Data were obtained from wrist-worn accelerometers used by 4551 participants on a single day from 6:00 am to 10:00 pm. The accelerometers recorded minute-by-minute activity generating 960 separate measures for each participant. I extracted principal components representing the 960 minute variables using the _PCA_ function in the _FactoMineR_ package and examined the loading vectors to determine the predominant features. To determine if activity is predictive of subject age, I divide the data into training and test sets using an 80/20 splint and then constructed an OLS model using the principal component scores as predictors. Component selection was performed using 10-fold cross-validation using mean square error of prediction (MSEP) to pick the optimum number of components to retain. The final model was compared with lasso regression applied to the original accelerometer data. 
