# URL-predication-using-Machine-leaning-Model
URL predication using Machine leaning Model

The provided Jupyter notebook is designed for detecting spam URLs using a machine learning model. Below is a summary suitable for a GitHub repository description in a beginner-friendly format.

---

#Spam URL Detection Using Machine Learning

This project demonstrates how to build a machine learning model to detect spam URLs. The steps include data preprocessing, exploratory data analysis (EDA), feature engineering, and model training and evaluation. Here's an overview of the process:

 1.Data Loading and Preprocessing
- Loading Libraries: The necessary libraries such as NumPy, pandas, matplotlib, seaborn, plotly, and scikit-learn are imported.
- Loading Data: The dataset is loaded using pandas.
- Data Inspection: The first few rows and the shape of the dataset are inspected to understand its structure.
- Missing Values and Duplicates:** Checks for missing values and duplicate entries, and removes duplicates to ensure data quality.

#2. Exploratory Data Analysis (EDA)
- Class Distribution: The distribution of spam and legitimate URLs is visualized using a pie chart.
- Feature Creation: New features are created from the URLs, such as:
  - Length of the URL
  - Presence of the word "subscribe"
  - Presence of a hash (#) symbol
  - Number of digits in the URL
  - Whether the URL uses HTTPS
  - Number of words in the URL

#3. Data Visualization
- Histogram: A histogram is created to visualize the length of URLs, categorized by spam and non-spam.

#4. Model Training
- Feature Selection: Relevant features are selected for training the model.
- Data Splitting: The data is split into training and testing sets.
- Scaling and Model Pipeline: A pipeline is created using MinMaxScaler for scaling the features and DecisionTreeClassifier for classification.
- Model Training: The model is trained on the training data.

#5. Model Evaluation
- ROC Curve: The ROC curve is plotted to evaluate the model's performance.
- Metrics: The ROC-AUC score, accuracy, and classification report (precision, recall, F1-score) are printed.

#6. Prediction
- User Input: The model accepts a URL input from the user and predicts whether it is spam or legitimate based on the trained model.

### Example Usage
url = "https://example.com/subscribe-now"
prediction = clf.predict(input_data_reshaped)
if prediction[0] == 1:
    print("Spam URL")
else:
    print("Legitimate URL")
```

This project is a practical demonstration of how machine learning can be applied to cybersecurity tasks such as spam detection. The code is structured to be easily understandable for beginners.
