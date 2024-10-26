**Credit Card Routing Predictive Model:**

**Project Overview:**
This project is designed to develop a predictive model for optimizing the routing of credit card transactions through various Payment Service Providers (PSPs) in the DACH region (Germany, Switzerland, Austria). The model minimizes transaction fees and failures using historical transaction data and advanced machine learning techniques.

**Repository Structure:**
├── data/
│   ├── raw/                        # Raw data files (PSP_Jan_Feb_2019.xlsx)
│   └── processed/                  # Processed data files (processed_transactions.csv)
├── reports/                        # Analysis results, plots, and model outputs
│   ├── .png files                  # Plots for model evaluation and comparison
│   └── .txt files                  # Final evaluation metrics and business insights
├── credit_card_routing_model.ipynb  # Main Jupyter notebook for the project
├── README.md                       # Project overview and setup instructions
├── requirements.txt                # Required packages and dependencies

**How to Run the Project:**

**1. Clone the repository:**

git clone https://github.com/Ahsan97Javed/credit-card-routing-model

**2. Install dependencies:** 
Run the following command in the root directory of the project to install all required packages:

pip install -r requirements.txt

**3. Run the Jupyter Notebook:** 
Open the credit_card_routing_model.ipynb file in Jupyter Notebook or JupyterLab to execute the code. The notebook contains sections for data exploration, model building, hyperparameter tuning, and evaluation.

**4. Data:**
The raw transaction data can be found in the data/raw/ folder.
The processed data will be automatically saved in data/processed/ during the notebook execution.

**5. Reports:**
All key visualizations and model evaluation results will be saved in the reports/ folder.
Summary reports are available in text files and include key model performance metrics such as accuracy, precision, recall, and F1-score.

**Key Features:**
Data Preparation: Data cleaning, feature selection, and handling of class imbalance using SMOTE.
Modeling: Logistic Regression, Random Forest, Stacking Classifier.
Hyperparameter Tuning: GridSearchCV and RandomizedSearchCV for model optimization.
Evaluation: Confusion matrix, classification report, and model performance comparison.

**Results:**
Best Performing Model: Random Forest with selected features, achieving an accuracy of 80.82%.
Cost Optimization: Simplecard identified as the most cost-effective PSP.

**Business Implications:**
The predictive model helps businesses reduce transaction fees by selecting the optimal PSP based on past transaction success rates and costs.

**Future Improvements:**
Further fine-tuning of the model to handle class imbalance more effectively.
Integration of additional business features (e.g., transaction geography, customer profiles) to improve model precision.
