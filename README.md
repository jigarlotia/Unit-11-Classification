# Unit-11-Risky Business Homework (Classifications Unit)

This unit uses several machine learning models to predict credit risk using the data provided.  Since credit is inherently imbalanced i.e. number of good loans are much higher than the number of at-risk loans, this homework focuses on using the imbalanced classes to evaluate the models.

The Homework consists of 2 main techniques that are explored:
- Resampling
- Ensemble Learning


## Resampling

The resampling is covered in this [notebook](credit_risk_resampling.ipynb) and uses the Lending Club data from [lending_data.csv](Resources/lending_data.csv) and then on the data applies:
- Basic Label Encoding using `LabelEncoder`.

- Data is scaled using the `StandardScaler` and split into training and testing data.

- Oversample the data using the `Naive Random Oversampler` and `SMOTE` algorithms.

- Undersample the data using the `Cluster Centroids` algorithm.

- Over- and undersample using a combination `SMOTEENN` algorithm.

And for each of the above :   
- `Balanced accuracy score` is calculated.

- `Confusion Matrix` is generated.

- `Imbalanced Classification Report` is printed.

Using the above metrix, best model is identified.

## Ensemble Learning

The Ensemble Learning is covered in this [notebook](credit_risk_ensemble.ipynb) and uses the Quaterly Lending Club data for 2019 from [LoanStats_2019Q1.csv](Resources/LoanStats_2019Q1.csv) and then on the data applies:
- Basic Label Encoding using `LabelEncoder`.

- Data is scaled using the `StandardScaler` and split into training and testing data.

- Data is trained using the `Balanced Random Forest Classifier` and `Easy Ensemble classifier` algorithms.


And for each of the above algorithms:   
- `Balanced accuracy score` is calculated.

- `Confusion Matrix` is generated.

- `Imbalanced Classification Report` is printed.

Using the above metrix, best model is identified.