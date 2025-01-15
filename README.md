# Bank Marketing Campaign Prediction

## 📄 Problem Statement

This project analyzes the direct marketing campaigns of a banking institution. These campaigns involved phone calls, often requiring multiple contacts to determine if a client would subscribe to a bank term deposit.

The goal is to develop a machine learning model to predict whether a client will subscribe to a bank term deposit (`yes`/`no`), based on campaign-related data.

---

## 🧠 Project Approach

### 1. **Data Exploration**

- Understanding the dataset, its 21 features, and identifying patterns or correlations.
- Discarded the output column (`y`) initially to explore independent variables.

### 2. **Feature Engineering**

- Cleaned and preprocessed the data to handle missing values and outliers.
- Selected the most relevant independent variables to enhance prediction accuracy.

### 3. **Building Samples**

- Split the dataset into training, validation, and test samples for robust model evaluation.

### 4. **Model Selection**

- Evaluated the following classifiers:
  - **SGD**: Stochastic Gradient Descent (used once as a baseline and once with optimized hyperparameters).
  - **RF**: Random Forest (used once as a baseline and once with optimized hyperparameters).
  - **GB**: Gradient Boosting (used once as a baseline and once with optimized hyperparameters).

### 5. **Model Evaluation**

- Assessed model performance using metrics like accuracy, precision, recall, and F1-score.
- Optimized the hyperparameters for the best-performing model.

---

## 🔿 Project Goals

The primary objective is to predict whether a client will subscribe to a bank term deposit (`yes`/`no`) by leveraging data-driven insights. The secondary goal is to identify key features influencing customer behavior and use these insights to optimize marketing strategies.

---

## 🏆 Results and Key Insights

- **Best Model**: Gradient Boosting Classifier, achieving:

  - **Accuracy**: 79.5%
  - **Precision**: 0.82
  - Identified 62% of potential subscribers.

- **Key Features**:

  - **Consumer Price Index (`cons.price.idx`)**: High values positively influenced subscriptions.
  - **Euribor 3-month Rate (`euribor3m`)**: High values were a strong indicator for subscriptions.

- **Business Insight**:

  - Targeting customers with high `cons.price.idx` and `euribor3m` values can enhance the campaign's efficiency by focusing on high-potential clients, saving resources, and driving growth.

---

## 🔧 Tools and Technologies

- **Programming Language**: Python
- **Libraries Used**:
  - Data Manipulation: Pandas, NumPy
  - Data Visualization: Matplotlib, Seaborn
  - Machine Learning: Scikit-learn
- **Environment**: Jupyter Notebook

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bank-marketing-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd bank-marketing-prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the notebook to explore and test the model:
   ```bash
   jupyter notebook
   ```

---

## 📚 Dataset

- The dataset contains 21 features, including:
  - Client attributes: `age`, `job`, `marital`, `education`, etc.
  - Campaign details: `campaign`, `previous`, `pdays`, etc.
  - Economic indicators: `cons.price.idx`, `euribor3m`, etc.
- Output: `y` (target variable indicating subscription).

---

## 🛠️ Future Enhancements

- Explore additional algorithms to further improve performance.
- Integrate real-time prediction APIs for deployment.
- Analyze regional or demographic trends to tailor marketing efforts.

---

## 🤝 Acknowledgments

Thanks to the dataset providers for enabling this analysis. This project demonstrates how data-driven decision-making can revolutionize marketing strategies in the banking industry.

---

