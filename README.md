<h1 align="center">🏦 <b>Bank Customer Churn Prediction</b></h1>
<h2>📖 <b>Overview</b></h2>

Customer churn occurs when customers stop doing business with a company. In the banking sector, churn often shows up as inactivity or disengagement — like fewer transactions or reduced account balances.

This project predicts whether a customer will churn or stay using Artificial Neural Networks (ANN) and H2O AutoML. The results help identify high-risk customers and guide retention strategies.

<h2>🎯 <b>Objectives</b></h2>

🧩 Identify and visualize key factors contributing to customer churn

🤖 Build a classification model to predict customer churn

📊 Attach probability scores to each prediction for targeted retention efforts

⚖️ Compare performance between ANN and H2O AutoML models

<h2>🧾 <b>Dataset</b></h2>

Source: Churn_Modelling.csv

Description: Contains details of bank customers such as credit score, geography, balance, and churn status.

Key Features:

CreditScore, Age, Balance, EstimatedSalary

Geography, Gender, NumOfProducts

Exited (Target variable: 1 = Churned, 0 = Retained)

<h2>⚙️ <b>Project Workflow</b></h2> <h3>1️⃣ Data Preprocessing</h3>

Removed irrelevant columns (CustomerId, RowNumber, Surname)

Encoded categorical variables (Geography, Gender)

Scaled numeric features using StandardScaler

<h3>2️⃣ Exploratory Data Analysis (EDA)</h3>

Visualized churn rates using bar plots and histograms

Explored correlations between features

Compared churn rates across age, gender, and geography

<h3>3️⃣ Model Building – ANN</h3>

Built a Neural Network using TensorFlow/Keras

Hidden layers use ReLU, output uses Sigmoid activation

Optimized using Adam and Binary Cross-Entropy loss

<h3>4️⃣ Model Building – H2O AutoML</h3>

Used H2O AutoML to automatically train and tune multiple ML models

Compared models (GBM, XGBoost, Deep Learning, etc.)

Selected the top-performing model based on AUC and accuracy

<h3>5️⃣ Model Evaluation</h3>

Metrics used for evaluation:

✅ Accuracy

✅ Precision

✅ Recall

✅ F1 Score

✅ AUC-ROC Curve

<h2>🧰 <b>Technologies & Libraries</b></h2>
Category	Tools / Libraries
Language	Python
Environment	Google Colab
Data Handling	Pandas, NumPy
Visualization	Matplotlib, Seaborn
Modeling	TensorFlow, Keras, H2O.ai
Preprocessing	scikit-learn
<h2>📊 <b>Results</b></h2>

Both ANN and H2O AutoML showed strong predictive performance.

H2O AutoML achieved slightly better accuracy due to automatic hyperparameter tuning.

Probability outputs help identify and target customers most likely to churn.

<h2>📁 <b>Project Structure</b></h2>

📦 Bank_Customer_Churn_Prediction
 ┣ 📂 data
 ┃ ┗ 📄 Churn_Modelling.csv
 ┣ 📂 notebooks
 ┃ ┗ 📄 Bank_customer_churn_pred.ipynb
 ┣ 📂 results
 ┃ ┗ 📄 model_performance.csv
 ┣ 📄 README.md
 ┗ 📄 requirements.txt


<h2>🚀 <b>Future Enhancements</b></h2>

🌐 Deploy model using Flask or Streamlit for real-time churn prediction

🧩 Integrate predictions into CRM systems for proactive alerts

📈 Use SHAP or LIME for model explainability

⚙️ Experiment with ensemble and hybrid models for improved performance

<h2>👩‍💻 <b>Author</b></h2>

Vaishnavi Chaughule
