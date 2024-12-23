## Heart Disease Prediction Model

This repository contains a fully developed heart disease prediction model of which the features
that were utilized consist of various health-related data of an individual. The processes that
were followed to develop this model included the exploration of data distribution of some 
features and their relationship amongst themselves, the exploration of the correlation between
the attributes to determine which features have weak correlation amongst themselves so that they
can be dropped if possible, and the implementation of the model itself.

### Features
The dataset that was utilized did not contain any null values but there was only one duplicate of 
which the record was dropped to avoid any impact it could have potentially had. The type 
of model that was utilized for this classification case is the logistic regression, there was 
no scaling of features that took place, every data point was used as it was. All the features 
were in numerical form so there was no need for data transformation.

### Dataset
Health data of individuals was utilized to develop this model, the attributes utilized can be seen below.
- **age**
- **sex**
- **cp**
- **trestbps**
- **chol**
- **fbs**
- **restecg**
- **thalach**
- **exang**
- **oldpeak**
- **slope**
- **ca** 
- **thal** 
- **target** 

### Requirements
To run the project, ensure you have the following installed:

- **Python 3.8+**
- **Libraries**
  - **pandas**
  - **numpy**
  - **matplotlib**
  - **seaborn**
  - **scikit-learn**

### Results
The variables of the dataset are utilized as features except the “target” variable which is 
the variable that will be predicted by the trained model. The target is already encoded as 
0s and 1s, of which 0 is assumed to indicate no heart disease and 1 indicates a heart disease.
Hence this is a classification task, **logistic regression** is utilized to construct this model, 
and the data has been split into 80% training data and 20% testing data. Post the training of 
the model, an accuracy of the model stands at 85.25% when predicting presence of a heart disease
based on the data that it was not trained with.

The features that were utilized to construct this model proved their strong importance 
individually as they produced a model with an accuracy of 85.25%. There were features 
with weak correlation with the target but for simplicity, no features were dropped and a 
quality model with an excellent accuracy was produced.

### Future Work
  - Incorporate various kinds of features to strengthen the accuracy of the model
  - Explore various kinds of modeling techniques with an intention to increase the accuracy of the model.
  - Integrate the model into a web application for real-time predictions.

