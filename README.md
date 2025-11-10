<h1 align="center">🏦 Bank Customer Churn Prediction System</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/ANN_Accuracy-86.2%25-success.svg" alt="ANN Accuracy">
  <img src="https://img.shields.io/badge/H2O_AutoML-Stacked_Ensemble-orange.svg" alt="H2O AutoML">
  <img src="https://img.shields.io/badge/Dataset-10K_Records-informational.svg" alt="Dataset">
  <img src="https://img.shields.io/badge/Status-Complete-brightgreen.svg" alt="Status">
</p>

<h2>🎯 Overview</h2>
<p>Banks lose approximately 20% of their customers annually to churn, resulting in millions in lost revenue and increased acquisition costs. Traditional reactive approaches to customer retention are costly and inefficient, often addressing churn only after customers have already decided to leave. This project tackles this critical business challenge by building an intelligent predictive system that identifies at-risk customers before they churn, enabling proactive, data-driven retention campaigns.</p>
<p>Using machine learning on 10,000 customer records with 14 behavioral and demographic features, the system compares two approaches: a custom Artificial Neural Network (ANN) achieving <b>86.2% accuracy</b> and H2O AutoML's Stacked Ensemble model. The solution provides <b>real-time churn probability scores</b> for targeted interventions, allowing banks to focus retention efforts on high-value, high-risk customer segments with precision.</p>

<h2>💡 The Problem</h2>
<p>Customer churn represents a critical challenge for financial institutions:</p>
<ul>
<li><b>Revenue Loss:</b> 20% annual customer attrition directly impacts profitability</li>
<li><b>High Acquisition Costs:</b> Acquiring new customers costs 5-25x more than retaining existing ones</li>
<li><b>Reactive Strategies:</b> Traditional retention efforts occur too late in the customer lifecycle</li>
<li><b>Untargeted Campaigns:</b> Blanket retention strategies waste resources on low-risk customers</li>
<li><b>Hidden Patterns:</b> Complex churn indicators buried in customer behavior data remain undetected</li>
</ul>

<h2>✨ The Solution</h2>
<p>An intelligent churn prediction system that:</p>
<ul>
<li>Analyzes 14 customer attributes to identify hidden churn patterns and risk factors</li>
<li>Achieves 86.2% accuracy with deep learning, enabling reliable early-warning detection</li>
<li>Provides probability-based risk scoring for each customer, not just binary predictions</li>
<li>Enables targeted retention campaigns focused on high-risk, high-value customer segments</li>
<li>Automates model selection through H2O AutoML, comparing 10+ algorithms systematically</li>
<li>Identifies key predictors (age, geography, balance-salary ratio) for strategic interventions</li>
</ul>

<h2>📊 Key Results & Business Impact</h2>

<table>
<tr>
<th>Metric</th>
<th>ANN Model</th>
<th>H2O AutoML</th>
<th>Business Value</th>
</tr>
<tr>
<td><b>Accuracy</b></td>
<td>86.2%</td>
<td>Ensemble (10 models)</td>
<td>Reliable churn prediction for strategic planning</td>
</tr>
<tr>
<td><b>Dataset Size</b></td>
<td colspan="2">10,000 records</td>
<td>Statistically robust for banking applications</td>
</tr>
<tr>
<td><b>Features Analyzed</b></td>
<td colspan="2">14 attributes</td>
<td>Comprehensive customer behavior profiling</td>
</tr>
<tr>
<td><b>Feature Engineering</b></td>
<td colspan="2">2 derived features</td>
<td>BalanceSalaryRatio & TenureByAge for deeper insights</td>
</tr>
<tr>
<td><b>Models Compared</b></td>
<td>1 (ANN)</td>
<td>10+ algorithms</td>
<td>Systematic evaluation ensures optimal selection</td>
</tr>
<tr>
<td><b>Prediction Type</b></td>
<td colspan="2">Probability scores</td>
<td>Risk-based customer segmentation for targeted campaigns</td>
</tr>
</table>

<h3>🔬 Model Comparison & Selection</h3>

<table>
<tr>
<th>Approach</th>
<th>Method</th>
<th>Key Advantages</th>
<th>Performance</th>
</tr>
<tr>
<td><b>Custom ANN</b></td>
<td>Keras Neural Network</td>
<td>Fine-tuned architecture, interpretable layers, fast inference</td>
<td>86.2% accuracy</td>
</tr>
<tr>
<td><b>H2O AutoML</b></td>
<td>Stacked Ensemble</td>
<td>Automated hyperparameter tuning, combines 10+ models, optimal performance</td>
<td>Best overall (leaderboard)</td>
</tr>
</table>

<h3>📈 Key Findings from Analysis</h3>

<pre><code>Churn Distribution:
- Churned customers: ~20% of total
- Retained customers: ~80% of total

Top Churn Predictors (from EDA):
- Age: Older customers show higher churn rates
- Geography: Germany exhibits elevated churn compared to France/Spain
- Gender: Female customers demonstrate slightly higher churn
- IsActiveMember: Inactive members are significantly more likely to churn
- NumOfProducts: Customers with 3-4 products show unusual churn patterns

Engineered Features Impact:
- BalanceSalaryRatio: Strong predictor - high ratios correlate with retention
- TenureByAge: Reveals lifecycle patterns - shorter relative tenure increases risk
</code></pre>

<h3>🎯 Business Applications</h3>

<p><b>Probability-Based Customer Segmentation:</b></p>
<ul>
<li><b>High Risk (>70% churn probability):</b> Immediate personalized intervention, dedicated account manager</li>
<li><b>Medium Risk (40-70%):</b> Targeted retention offers, engagement campaigns</li>
<li><b>Low Risk (<40%):</b> Standard service, monitor for changes</li>
</ul>

<h2>🔍 Dataset & Features</h2>

<h3>Data Overview</h3>
<ul>
<li><b>Source:</b> Churn_Modelling.csv</li>
<li><b>Size:</b> 10,000 customer records</li>
<li><b>Features:</b> 14 attributes (after preprocessing)</li>
<li><b>Target:</b> Binary classification (0 = Retained, 1 = Churned)</li>
<li><b>Class Distribution:</b> Imbalanced (~20% churn, ~80% retention)</li>
</ul>

<h3>Feature Categories</h3>

<table>
<tr>
<th>Category</th>
<th>Features</th>
<th>Business Relevance</th>
</tr>
<tr>
<td><b>Demographic</b></td>
<td>Age, Gender, Geography</td>
<td>Customer profile and location-based patterns</td>
</tr>
<tr>
<td><b>Financial</b></td>
<td>CreditScore, Balance, EstimatedSalary</td>
<td>Economic capacity and creditworthiness indicators</td>
</tr>
<tr>
<td><b>Behavioral</b></td>
<td>Tenure, NumOfProducts, HasCrCard, IsActiveMember</td>
<td>Customer engagement and product adoption patterns</td>
</tr>
<tr>
<td><b>Engineered</b></td>
<td>BalanceSalaryRatio, TenureByAge</td>
<td>Advanced relationship metrics for deeper insights</td>
</tr>
<tr>
<td><b>Target</b></td>
<td>Exited</td>
<td>Churn status (0 = retained, 1 = churned)</td>
</tr>
</table>

<h3>Feature Engineering Rationale</h3>

<p><b>BalanceSalaryRatio = Balance / EstimatedSalary</b></p>
<ul>
<li>Captures wealth accumulation relative to income</li>
<li>High ratios suggest financial stability → lower churn risk</li>
<li>Low ratios may indicate financial stress → retention opportunity</li>
</ul>

<p><b>TenureByAge = Tenure / Age</b></p>
<ul>
<li>Normalizes tenure by customer age (lifecycle stage)</li>
<li>Young customers with short tenure = normal; older customers = warning signal</li>
<li>Reveals lifecycle-adjusted engagement patterns</li>
</ul>

<h2>⚙️ Technical Implementation</h2>

<h3>End-to-End ML Pipeline</h3>

<h4>1️⃣ Data Acquisition & Exploration</h4>
<ul>
<li>Loaded 10,000 customer records from Google Drive (Colab environment)</li>
<li>Initial inspection: 14 features + 3 identifier columns (CustomerId, RowNumber, Surname)</li>
<li>Verified data integrity: <b>zero missing values</b> across all features</li>
<li>Analyzed target distribution: identified 20% churn rate (class imbalance)</li>
</ul>

<h4>2️⃣ Exploratory Data Analysis</h4>
<ul>
<li>Visualized churn distribution with pie chart (80/20 split)</li>
<li>Generated countplots for categorical features (Geography, Gender, HasCrCard, IsActiveMember) segmented by churn status</li>
<li>Created boxplots for continuous features (CreditScore, Age, Tenure, Balance, NumOfProducts, EstimatedSalary) to identify distributions and outliers</li>
<li>Plotted tenure histogram comparing churned vs retained customers</li>
<li>Identified key patterns: age and geography emerge as strong churn predictors</li>
</ul>

<h4>3️⃣ Feature Engineering & Preprocessing</h4>
<ul>
<li>Dropped non-predictive identifiers: CustomerId, RowNumber, Surname</li>
<li>Engineered 2 derived features:
<ul>
<li><b>BalanceSalaryRatio:</b> Wealth accumulation indicator via EDA visualization validation</li>
<li><b>TenureByAge:</b> Lifecycle-normalized engagement metric</li>
</ul>
</li>
<li>Encoding strategy:
<ul>
<li><b>Label Encoding:</b> Gender (Male=1, Female=0)</li>
<li><b>One-Hot Encoding:</b> Geography (3 dummy variables: France, Germany, Spain)</li>
</ul>
</li>
<li>Feature scaling: MinMaxScaler on 6 continuous variables (Tenure, CreditScore, Age, Balance, NumOfProducts, EstimatedSalary)</li>
<li>Train-test split: 80/20 stratified split (8,000 train / 2,000 test), random_state=5</li>
</ul>

<h4>4️⃣ Model Development – Artificial Neural Network</h4>
<ul>
<li>Framework: TensorFlow 2.x with Keras Sequential API</li>
<li>Architecture:
<ul>
<li><b>Input Layer:</b> 14 features (after encoding and engineering)</li>
<li><b>Hidden Layer 1:</b> 12 neurons, ReLU activation</li>
<li><b>Hidden Layer 2:</b> 6 neurons, ReLU activation</li>
<li><b>Output Layer:</b> 1 neuron, Sigmoid activation (binary classification)</li>
</ul>
</li>
<li>Compilation:
<ul>
<li><b>Optimizer:</b> Adam (adaptive learning rate)</li>
<li><b>Loss Function:</b> Binary Cross-Entropy</li>
<li><b>Metrics:</b> Accuracy</li>
</ul>
</li>
<li>Training: 100 epochs on 8,000 training samples</li>
<li>Evaluation: Confusion matrix, classification report, accuracy score on 2,000 test samples</li>
<li><b>Result:</b> 86.2% test accuracy</li>
</ul>

<h4>5️⃣ Model Development – H2O AutoML</h4>
<ul>
<li>Framework: H2O.ai AutoML (automated machine learning)</li>
<li>Configuration:
<ul>
<li><b>max_runtime_secs:</b> 300 seconds (5 minutes)</li>
<li><b>max_models:</b> 10 algorithms trained and tuned</li>
<li><b>seed:</b> 10 (reproducibility)</li>
<li><b>nfolds:</b> 2 (cross-validation)</li>
<li><b>verbosity:</b> info (detailed logging)</li>
</ul>
</li>
<li>Preprocessing: H2O automatically handles encoding and feature transformations</li>
<li>Model types explored: GBM, XGBoost, Deep Learning, GLM, Random Forest, Stacked Ensembles</li>
<li>Leaderboard ranking by AUC, accuracy, and other metrics</li>
<li><b>Best Model:</b> Stacked Ensemble (combines top 10 models)</li>
<li>Output: Probability predictions for risk-based customer segmentation</li>
</ul>

<h4>6️⃣ Model Evaluation & Comparison</h4>
<ul>
<li>ANN evaluation metrics:
<ul>
<li>Accuracy: 86.2%</li>
<li>Confusion matrix visualization (heatmap)</li>
<li>Classification report (precision, recall, F1-score per class)</li>
</ul>
</li>
<li>H2O AutoML evaluation:
<ul>
<li>Leaderboard comparison across 10+ models</li>
<li>Stacked Ensemble selected as best performer</li>
<li>Model performance tested on holdout set</li>
<li>Probability outputs for business segmentation</li>
</ul>
</li>
<li>Decision: H2O AutoML chosen for production due to superior generalization and automatic optimization</li>
</ul>

<h2>🛠️ Technologies & Tools</h2>

<h3>Core Stack</h3>
<ul>
<li><b>Python 3.8+</b> - Primary programming language</li>
<li><b>Google Colab</b> - Cloud-based Jupyter environment with GPU support</li>
<li><b>Pandas</b> - Data manipulation and preprocessing</li>
<li><b>NumPy</b> - Numerical computations</li>
</ul>

<h3>Deep Learning & AutoML</h3>
<ul>
<li><b>TensorFlow 2.x / Keras</b> - Neural network implementation</li>
<li><b>H2O.ai</b> - Automated machine learning platform</li>
<li><b>H2O AutoML</b> - Automatic model selection and hyperparameter tuning</li>
</ul>

<h3>Preprocessing & Evaluation</h3>
<ul>
<li><b>scikit-learn</b> - MinMaxScaler, train_test_split, accuracy_score, confusion_matrix, classification_report</li>
</ul>

<h3>Visualization & Analysis</h3>
<ul>
<li><b>Matplotlib</b> - Statistical plotting (histograms, pie charts)</li>
<li><b>Seaborn</b> - Advanced visualizations (countplot, boxplot, heatmap)</li>
</ul>

<h3>Neural Network Architecture</h3>
<ul>
<li><code>keras.Sequential</code> - Sequential model building</li>
<li><code>keras.layers.Dense</code> - Fully connected layers</li>
<li><b>Activation functions:</b> ReLU (hidden layers), Sigmoid (output layer)</li>
<li><b>Optimizer:</b> Adam with binary cross-entropy loss</li>
</ul>

<h3>H2O AutoML Algorithms Explored</h3>
<ul>
<li><code>StackedEnsemble</code> - Meta-model combining predictions (selected)</li>
<li><code>GBM</code> - Gradient Boosting Machine</li>
<li><code>XGBoost</code> - Extreme Gradient Boosting</li>
<li><code>DeepLearning</code> - H2O's neural network implementation</li>
<li><code>GLM</code> - Generalized Linear Model</li>
<li><code>RandomForest</code> - Ensemble of decision trees</li>
<li><code>DRF</code> - Distributed Random Forest</li>
</ul>

<h2>🚀 Getting Started</h2>

<h3>Prerequisites</h3>

<pre><code>Python 3.8 or higher
Google Colab account (recommended) or local Jupyter environment
Google Drive (for dataset storage in Colab setup)
</code></pre>

<h3>Installation</h3>

<pre><code># Clone the repository
git clone https://github.com/yourusername/bank-churn-prediction.git
cd bank-churn-prediction

# Install core dependencies
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow

# Install H2O AutoML
pip install requests tabulate colorama future h2o

# Verify installations
python -c "import tensorflow as tf; print(f'TensorFlow: {tf.__version__}')"
python -c "import h2o; print(f'H2O: {h2o.__version__}')"
</code></pre>

<h3>Running the Project</h3>

<h4>Option 1: Google Colab (Recommended)</h4>

<pre><code># 1. Upload Churn_Modelling.csv to your Google Drive
# 2. Open Bank_customer_churn_pred.ipynb in Google Colab
# 3. Mount Google Drive when prompted
# 4. Run all cells sequentially

# Mount Drive (first cell in notebook)
from google.colab import drive
drive.mount('/content/drive')
</code></pre>

<h4>Option 2: Local Jupyter</h4>

<pre><code># Ensure dataset is in correct path
# Update file path in notebook: df = pd.read_csv("path/to/Churn_Modelling.csv")

# Launch Jupyter Notebook
jupyter notebook Bank_customer_churn_pred.ipynb

# Or run with JupyterLab
jupyter lab
</code></pre>

<h3>Project Structure</h3>

<pre><code>bank-churn-prediction/
├── Bank_customer_churn_pred.ipynb  # Main ML pipeline notebook
├── Churn_Modelling.csv             # Customer data (10K records, 14 features)
├── README.md                       # Project documentation
 
</code></pre>

<h2>📋 Methodology Highlights</h2>

<h3>Why This Approach Works</h3>

<table>
<tr>
<th>Design Decision</th>
<th>Rationale</th>
<th>Business Impact</th>
</tr>
<tr>
<td><b>Feature Engineering</b></td>
<td>Created BalanceSalaryRatio & TenureByAge through EDA insights</td>
<td>Uncovered hidden patterns not visible in raw features</td>
</tr>
<tr>
<td><b>Dual Modeling Strategy</b></td>
<td>ANN for interpretability, AutoML for optimal performance</td>
<td>Balance between transparency and accuracy for stakeholders</td>
</tr>
<tr>
<td><b>Probability Outputs</b></td>
<td>Risk scores instead of binary predictions</td>
<td>Enables nuanced customer segmentation and resource allocation</td>
</tr>
<tr>
<td><b>H2O AutoML</b></td>
<td>Automated hyperparameter tuning across 10+ algorithms</td>
<td>Maximizes performance without manual experimentation overhead</td>
</tr>
<tr>
<td><b>Stratified Splitting</b></td>
<td>Preserves class distribution in train/test sets</td>
<td>Ensures reliable evaluation on imbalanced churn data</td>
</tr>
<tr>
<td><b>Comprehensive EDA</b></td>
<td>Visual analysis before modeling</td>
<td>Identifies key predictors (age, geography) for strategic focus</td>
</tr>
</table>

<h2>🎯 Real-World Applications</h2>

<h3>Banking Use Cases</h3>
<ul>
<li><b>Proactive Retention Campaigns:</b> Target high-risk customers with personalized offers before they churn</li>
<li><b>Resource Optimization:</b> Focus retention budget on customers most likely to respond positively</li>
<li><b>Customer Segmentation:</b> Risk-stratified groups for differentiated service strategies</li>
<li><b>Predictive Analytics Dashboard:</b> Real-time churn risk monitoring for account managers</li>
<li><b>A/B Testing:</b> Measure effectiveness of retention interventions by risk segment</li>
<li><b>Lifetime Value Optimization:</b> Combine churn probability with CLV for ROI-driven retention</li>
</ul>

<h3>Strategic Retention Interventions</h3>

<p><b>Age-Based Strategies (key predictor identified):</b></p>
<ul>
<li>Older customers: Retirement planning services, wealth management consultations</li>
<li>Middle-aged: Mortgage refinancing, education savings programs</li>
<li>Younger: Digital banking features, mobile app enhancements</li>
</ul>

<p><b>Geography-Based Strategies (Germany shows high churn):</b></p>
<ul>
<li>Localized product offerings tailored to German market preferences</li>
<li>Enhanced customer service in high-churn regions</li>
<li>Competitive analysis to match regional competitor offerings</li>
</ul>

<p><b>Engagement-Based Strategies (IsActiveMember predictor):</b></p>
<ul>
<li>Re-engagement campaigns for inactive members</li>
<li>Gamification and rewards for transaction activity</li>
<li>Personalized communication based on usage patterns</li>
</ul>

<h3>Deployment Considerations</h3>
<ul>
<li><b>Integration:</b> Connect predictions to CRM systems (Salesforce, HubSpot) for automated alerts</li>
<li><b>Batch Scoring:</b> Monthly churn risk assessment for entire customer base</li>
<li><b>Real-Time Scoring:</b> API endpoint for on-demand predictions during customer interactions</li>
<li><b>Model Monitoring:</b> Track prediction accuracy over time, retrain quarterly with fresh data</li>
<li><b>Explainability:</b> Use SHAP/LIME to explain individual predictions to retention teams</li>
<li><b>Compliance:</b> Ensure GDPR/data privacy compliance for customer data usage</li>
</ul>

<h2>🤝 Contributing</h2>
<p>Contributions are welcome! Whether you're interested in improving model performance, adding new features, expanding visualizations, or enhancing documentation, please feel free to:</p>
<ul>
<li>Fork the repository</li>
<li>Create a feature branch (<code>git checkout -b feature/improvement</code>)</li>
<li>Commit your changes (<code>git commit -m 'Add new feature'</code>)</li>
<li>Push to the branch (<code>git push origin feature/improvement</code>)</li>
<li>Open a Pull Request</li>
</ul>

<h2>📄 License</h2>
<p>This project is open source and available under the MIT License. See LICENSE file for details.</p>

<h2>⚠️ Disclaimer</h2>
<p>This project is designed for <b>educational and demonstration purposes</b>. Production deployment in banking environments requires additional considerations including regulatory compliance, data privacy (GDPR), model governance, bias auditing, and continuous monitoring. Always consult legal and compliance teams before deploying predictive models in customer-facing applications.</p>

<h2>👩‍💻 Author</h2>
<p><b>Vaishnavi Chaughule</b><br>Master's in Computer Science, Northeastern University<br>Specializing in machine learning applications for business intelligence and customer analytics</p>

<p align="center"><a href="https://github.com/vaishnavi1064">GitHub</a> • <a href="https://linkedin.com/in/vaishnavichaughule">LinkedIn</a> • <a href="mailto:vaishnavi10chaughule@gmail.com">Email</a></p>

<h2>🙏 Acknowledgments</h2>
<ul>
<li>Dataset source for providing realistic banking customer data for research purposes</li>
<li>TensorFlow and Keras communities for robust deep learning frameworks</li>
<li>H2O.ai for democratizing automated machine learning</li>
<li>Open-source Python data science ecosystem (Pandas, NumPy, scikit-learn, Matplotlib, Seaborn)</li>
</ul>

<p align="center"><i>If you find this project helpful, please consider giving it a ⭐️</i></p>
