# PCA-Analysis

### Research question: Which number of principal components should be used to determine the most important features that will help with undersstanding patient characteristics?

### Steps: 

#### 1.	Selecting the continuous variables to use in developing a model to understand patient characteristics.

#### 2.	Explore the original dataset and identify an initial dataset to use.

#### 3.	Standardize this initial dataset.

#### 4.	Compute a covariance matrix.

#### 5.	Review eigenvectors, eigenvalues, and scree plot to determine which variables are significant.

#### 6.	Determine the number of significant principal components.

#### Outcome: PCA was performed to determine the number of features that should be used when building a model.  The original dataset included 49 columns, with 22 of those columns being continuous.  I created the initial dataset by removing the columns that I didn't think would provide any value (Lat, Lng, population, and Item1 - Item8).  The removal of the columns left me with 11 features for my initial dataset.  I then standardized the dataset so I could calculate the covariance matrix.  Based on the cumulative sum of the explained variance ratio, two variables make up almost 34% of the variance and 9 variables make up 97%.  The scree plot starts plateauing at 8 with a slight increase from 8 to 9.  Therefore, I would reduce my dataset to use 8 out of the 11 principal components to reduce the dimensionality and likelihood of overfitting the model to understand patient characteristics.  Next steps will be to perform further analysis on categorical factors that would provide insight on patient characteristics not included in the PCA analysis.
