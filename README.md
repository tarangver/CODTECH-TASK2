# Description for Model Evaluation and Comparison

Name: TARANG VERMA

Company: CODTECH IT SOLUTIONS

ID: CT08DS1310

Domain: ARTIFICAL INTELLIGENCE

Duration: "25th MAY 2024 to 25th JUNE 2024

Description:

1. **Import Libraries**:
    - Import necessary libraries: `pandas`, `numpy`, `matplotlib.pyplot`, and several modules from `sklearn`.

2. **Load the Iris Dataset**:
    - Load the Iris dataset using `load_iris` from `sklearn.datasets`.
    - Extract features (X) and target labels (y) from the dataset.

3. **Split the Dataset**:
    - Use `train_test_split` from `sklearn.model_selection` to split the data into training and testing sets.
    - Set the test size to 30%, ensure stratified sampling by specifying `stratify=y`, and set a random state for reproducibility.

4. **Standardize the Features**:
    - Initialize `StandardScaler` from `sklearn.preprocessing`.
    - Fit the scaler on the training data and transform both the training and testing data to standardize the features.

5. **Initialize the Models**:
    - Create a dictionary of models with names as keys and corresponding model instances as values.
    - Models include: Logistic Regression, Decision Tree, Random Forest, SVM, and Neural Network.

6. **Train the Models and Make Predictions**:
    - Iterate over the dictionary of models.
    - Train each model on the standardized training data.
    - Make predictions on the testing data.
    - If the model supports probability predictions (`predict_proba`), also predict probabilities.

7. **Define a Function to Evaluate the Models**:
    - Create a function `evaluate_model` that calculates and returns various evaluation metrics:
        - Accuracy
        - Precision (weighted average)
        - Recall (weighted average)
        - F1 Score (weighted average)
        - ROC AUC (if probability predictions are available)

8. **Evaluate Each Model**:
    - Iterate over the results (predictions and probabilities) of each model.
    - Use the `evaluate_model` function to compute evaluation metrics for each model.
    - Store the evaluation results in a dictionary.

9. **Convert Evaluation Results to DataFrame**:
    - Convert the dictionary of evaluation results into a pandas DataFrame for easier comparison.
    - Print the DataFrame to display the evaluation metrics for each model.

10. **Plot the Evaluation Metrics**:
    - Use `plot` method on the DataFrame to create a bar plot of the evaluation metrics.
    - Set plot title, labels, and legend for clarity.
    - Rotate x-axis labels for better readability.
    - Display the plot using `plt.show()`.


The script loads the Iris dataset, splits it into training and testing sets, and standardizes the features. It then initializes five different machine learning models, trains them, and makes predictions. A custom evaluation function is defined to calculate accuracy, precision, recall, F1 score, and ROC AUC for each model. The results are compiled into a DataFrame and visualized using a bar plot, allowing for easy comparison of the models' performance.
