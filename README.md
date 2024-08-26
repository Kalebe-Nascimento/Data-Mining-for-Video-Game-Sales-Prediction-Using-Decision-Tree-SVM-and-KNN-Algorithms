# Data-Mining-for-Video-Game-Sales-Prediction-Using-Decision-Tree-SVM-and-KNN-Algorithms
This project focuses on predicting video game genres based on a comprehensive dataset of video game sales. We employ three machine learning algorithms: Decision Tree, Support Vector Machine (SVM), and K-Nearest Neighbors (KNN).
Introduction
This project focuses on predicting video game genres based on a comprehensive dataset of video game sales. We employ three machine learning algorithms: Decision Tree, Support Vector Machine (SVM), and K-Nearest Neighbors (KNN). The primary objective is to enhance prediction accuracy while maintaining computational efficiency.

Dataset
The dataset used in this project contains various attributes related to video games, such as:

Title: The name of the game.
Console: The platform on which the game was released.
Publisher: The company that published the game.
Developer: The company that developed the game.
Genre: The genre of the game (target variable).
Release Date: The date when the game was released.
Sales Figures: Total, NA, JP, PAL, and Other sales data.
Preprocessing Steps
Handling Missing Values: Numeric columns with missing values were filled with the mean value.
Encoding Categorical Variables: Categorical features (console, publisher, developer, and genre) were encoded using LabelEncoder to convert them into numerical format.
Feature Selection: SelectKBest was used to select the most relevant features for the classification task.
Data Balancing: SMOTE (Synthetic Minority Over-sampling Technique) was applied to balance the classes in the dataset.
Algorithms Used
Decision Tree: A model that uses a tree-like graph of decisions and their possible consequences. It is known for being easy to interpret but may overfit if not properly tuned.

Support Vector Machine (SVM): A powerful classifier that works by finding the hyperplane that best separates the classes in the feature space. The model was optimized using GridSearchCV for hyperparameter tuning.

K-Nearest Neighbors (KNN): A simple, instance-based learning algorithm that classifies a data point based on the majority label among its nearest neighbors. The optimal number of neighbors and weighting method were determined using GridSearchCV.

Model Evaluation
Cross-Validation: 5-fold cross-validation was used to evaluate the performance of each algorithm, ensuring that the models generalize well to unseen data.
Accuracy and Classification Reports: The accuracy of each model was reported, along with a detailed classification report that includes precision, recall, and F1-score for each genre.
Results
The performance of each algorithm was measured and compared, with the following average 5-fold cross-validation scores:

Decision Tree: Achieved a cross-validation score of 0.5291.
SVM: Achieved a cross-validation score of 0.0864.
KNN: Achieved a cross-validation score of 0.5083.
Conclusion
While the Decision Tree and KNN models showed moderate accuracy, the SVM model's performance was lower due to computational constraints and the complexity of the dataset. Future improvements may include further hyperparameter tuning, feature engineering, and experimenting with more advanced algorithms to enhance the prediction accuracy.

How to Run
Requirements: Ensure you have Python 3 installed along with the necessary libraries. You can install the required libraries using:

pip install -r requirements.txt

Running the Code: Execute the script using any Python IDE or run it in a Jupyter Notebook environment.
Exploring the Results: The script outputs the accuracy and classification reports for each model, allowing for a detailed comparison of their performance.
Future Work
Experiment with different feature selection methods.
Implement other machine learning algorithms like Random Forest or XGBoost.
Further optimize hyperparameters using more exhaustive search techniques.



Kalebe do Nascimento Sousa
Engineering student at Instituto Federal Fluminense
