# Movie-Genre-Classification
Objective:
To build a machine learning model that predicts the genre of a movie based on its plot summary (text description). This can help in automatically tagging or categorizing movies on streaming platforms or movie databases.
 Dataset Description:
Source: Berlin Movie Database (ftp://ftp.fu-berlin.de/pub/misc/movies/database/)

Files Provided:

train_data.txt: Contains labeled data in the format
ID ::: TITLE ::: GENRE ::: DESCRIPTION
test_data.txt: Contains unlabeled test data
ID ::: TITLE ::: DESCRIPTION
test_data_solution.txt: Contains the actual genre labels for the test data (used for evaluation).

Methodology:
Data Parsing:

Extracted the DESCRIPTION as the input feature and the GENRE as the label from training data.

Extracted only DESCRIPTION from test data for prediction.

Text Preprocessing:

Used TfidfVectorizer to convert raw text into numerical features using Term Frequency-Inverse Document Frequency (TF-IDF).

Model Training:

Trained multiple classifiers:

Logistic Regression

Naive Bayes (MultinomialNB)

Support Vector Machine (LinearSVC)

Prediction & Evaluation:

Predictions were made on the test dataset.

Evaluation used the actual genres from test_dat_solution.txt.

Metrics:

Accuracy

Precision, Recall, F1-Score

Confusion Matrix

Tools Used:
Python

Scikit-learn

Pandas

Matplotlib / Seaborn for visualization
