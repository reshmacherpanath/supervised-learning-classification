# supervised-learning-classification
This code imports the necessary libraries, loads the Iris dataset, splits it into training and testing sets, trains a logistic regression model, evaluates its accuracy, and then makes predictions on new samples.
Replace the new_samples array with your own data to predict the categories for different flowers.

Loading the Iris Dataset:

    The Iris dataset is loaded using datasets.load_iris().
    The features (Sepal Length, Sepal Width, Petal Length, Petal Width) are stored in X, and the target labels (Setosa, Versicolour, Virginica) are stored in y

Data Splitting:
        The dataset is split into a training set (X_train, y_train) and a test set (X_test, y_test) using train_test_split().
        The split is performed with 80% of the data used for training and 20% for testing. random_state is set for reproducibility.

Training the Logistic Regression Model:
        A logistic regression model is initialized using LogisticRegression().
        The model is trained on the training data using fit(X_train, y_train).

 Model Evaluation:
        The model's predictions are obtained on the test set using predict(X_test).
        The accuracy of the model is calculated by comparing the predicted labels (y_pred) to the actual labels (y_test) using accuracy_score().
        The accuracy is printed to the console.

Predicting New Samples:
        Three new flower samples are defined in the new_samples array, each with their Sepal Length, Sepal Width, Petal Length, and Petal Width values.
        The model is used to predict the class (Setosa, Versicolour, or Virginica) of each new sample using predict(new_samples).
        The predicted class labels are then mapped to their corresponding species names using iris.target_names.
        The results are printed to the console, showing the predicted species for each new sample.

This code provides a complete workflow for training a logistic regression model on the Iris dataset, evaluating its performance, and making predictions on new flower samples. 
You can replace the new_samples array with your own data to make predictions for different flowers
