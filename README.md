## KNN_IRIS_Dataset
## Preview of Data
## Introduction | kNN Algorithm
##### Statistical learning refers to a collection of mathematical and computation tools to understand data.In what is often called supervised learning, the goal is to estimate or predict an output based on one or more inputs.The inputs have many names, like predictors, independent variables, features, and variables being called common.The output or outputs are often called response variables, or dependent variables.If the response is quantitative – say, a number that measures weight or height, we call these problems regression problems.If the response is qualitative– say, yes or no, or blue or green, we call these problems classification problems.This case study deals with one specific approach to classification.The goal is to set up a classifier such that when it’s presented with a new observation whose category is not known, it will attempt to assign that observation to a category, or a class, based on the observations for which it does know the true category.This specific method is known as the k-Nearest Neighbors classifier, or kNN for short.Given a positive integer k, say 5, and a new data point, it first identifies those k points in the data that are nearest to the point and classifies the new data point as belonging to the most common class among those k neighbors.
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
