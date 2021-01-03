## KNN_IRIS_Dataset
## Preview of Data
##### There are 150 observations with 4 features each (sepal length, sepal width, petal length, petal width).
##### There are no null values, so we don't have to worry about that.
##### There are 50 observations of each species (setosa, versicolor, virginica).
## Split the dataset into a training set and a testing set
### Advantages
##### By splitting the dataset pseudo-randomly into a two separate sets, we can train using one set and test using another.
##### This ensures that we won't use the same observations in both sets.
##### More flexible and faster than creating a model using all of the dataset for training.
### Disadvantages
##### The accuracy scores for the testing set can vary depending on what observations are in the set.
##### This disadvantage can be countered using k-fold cross-validation.
## Notes
##### The accuracy score of the models depends on the observations in the testing set, which is determined by the seed of the pseudo-random number generator (random_state parameter).
##### As a model's complexity increases, the training accuracy (accuracy you get when you train and test the model on the same data) increases.
##### If a model is too complex or not complex enough, the testing accuracy is lower.
##### For KNN models, the value of k determines the level of complexity. A lower value of k means that the model is more complex.
### webApp For Iris Data Set: https://github.com/Furkan-Gulsen/iris_predictor_web_app
