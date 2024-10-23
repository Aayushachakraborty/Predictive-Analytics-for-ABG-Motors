# 🚗 Market Entry Analysis for ABG Motors in India

This project helps ABG Motors, a leading Japanese car manufacturer, in evaluating whether entering the Indian market will be a profitable decision. By analyzing car purchase patterns from sample data of two major cities—one in Japan and one in India—predictive analytics and classification models are used to forecast potential sales and determine market viability.

 📊 Project Overview

# Objective
The project aims to:
- Predict the likelihood of car purchases in the Indian market using data from Japanese operations.
- Forecast a minimum of 12,000 car sales in India over the course of a year to assess the market's profitability.
- Develop a classification model that predicts whether a customer will purchase a car based on demographic and behavioral data.

 📝 Data Processing & Model Building

# Data Preprocessing
- Datasets: The project uses two datasets representing customers from major cities in India and Japan. Columns include features like age, gender, income, car maintenance dates, and purchase status (Japanese dataset).
- Feature Engineering: Age and income were segmented into categories for a clearer analysis. A conversion from Japanese Yen to Indian Rupees was performed in the Japanese dataset to ensure comparable data.
- Binary Encoding: Gender was converted to numeric values (0 = Male, 1 = Female).
- Standardization: Income data was standardized for more effective model training.

# Predictive Modeling
A Logistic Regression model was used for the Japanese dataset to predict car purchases. The model’s coefficients were then applied to the Indian dataset to estimate purchase probabilities in the Indian market. Key features used:
1. Age Group
2. Gender
3. Income
4. Car Age Segment

# Model Results
- Japanese Dataset Accuracy: 69%
- ROC AUC Score: 0.75
- Feature Importance:
  - Car Age Segment: Highest influence
  - Income: Second-highest influence

# Forecasting Purchases
By applying the trained model from Japan to the Indian dataset, purchase probabilities were predicted for each customer. Customers with a probability greater than 0.2 were classified as potential car buyers.

# Insights
- Distribution of Purchase Predictions: Visualized through bar plots and pie charts to show the balance between predicted buyers and non-buyers.
- Purchase Probability Distribution: Histogram visualizations indicate the confidence level of the model's predictions.

# Business Outcome
The model estimates whether the target of 12,000 car sales can be achieved, providing ABG Motors with a data-backed decision to enter the Indian market.

 📂 Repository Structure
```
📦 ABG_Motors_Market_Entry
├── 📁 data                # Indian and Japanese datasets
├── 📁 notebooks           # Python notebooks for analysis and modeling
├── 📄 README.md           # Project overview and instructions
└── 📄 requirements.txt    # Dependencies for the project
```

 📊 Data Analysis & Visualization
The project leverages seaborn and matplotlib to generate insights:
- Box plots show the relationship between car age segments and income with purchase likelihood.
- Bar plots and pie charts help visualize purchase counts and probabilities.

 🚀 How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ABG_Motors_Market_Entry.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebooks to explore the analysis and model building:
   ```bash
   jupyter notebook
   ```

⚙️ Tech Stack
- Programming Language: Python
- Libraries: 
  - Data manipulation: `pandas`, `numpy`
  - Machine Learning: `scikit-learn`
  - Visualization: `matplotlib`, `seaborn`

 🛠 Future Improvements
- Incorporating more cities from both India and Japan to better generalize the model.
- Exploring more advanced machine learning algorithms like Random Forests or Gradient Boosting for better accuracy.


