# Fake News Classification - Accenture Team 1A

**Break Through Tech AI Studio - Fall 2025**

---

### 👥 **Team Members**

| Name | GitHub Handle | Contribution |
| :--- | :--- | :--- |
| **Steven Dong** | Feature engineering, model evaluation, and results analysis |
| **Koshish Shrestha** | Data cleaning pipeline, duplicate removal, EDA, Baseline Modeling |
| **Siying Lin** |  Exploratory Data Analysis (EDA), visualization, Sentiment Analysis, Modeling |
| **Ishita Gabhane** | EDA, Data Cleaning and performance metrics |
| **Xiomara Serpa** | Advanced modeling (Neural Networks) and hyperparameter tuning |
| **Chinyere Ugwuanyi** | Feature Engineering, EDA |

---

## 🎯 **Project Highlights**

* **High-Performance Classification:** Achieved **98.33% accuracy** using a Random Forest model with TF-IDF features, successfully distinguishing between real and fake news articles.
* **Business-Centric Solution:** Developed a scalable content moderation tool to support Accenture's Trust & Safety goals, mitigating legal liability and reputational risk.
* **Bias Mitigation:** Identified and removed a critical source of data leakage (the "Reuters" tag) which appeared in 99.8% of real news, ensuring the model learned linguistic patterns rather than source shortcuts.
* **Robust Preprocessing:** Implemented a rigorous cleaning pipeline that removed over 5,000 duplicate texts and handled empty content to ensure data quality.

---

## 👩🏽‍💻 **Setup and Installation**

# Fake News Classification - Accenture Team 1A

**Break Through Tech AI Studio - Fall 2025**

---

### 👥 **Team Members**

| Name | GitHub Handle | Contribution |
| :--- | :--- | :--- |
| **Steven Dong** | @[INSERT HANDLE] | Feature engineering, model evaluation, and results analysis |
| **Koshish Shrestha** | @[INSERT HANDLE] | Data cleaning pipeline, duplicate removal, and leakage prevention |
| **Siying Lin** | @[INSERT HANDLE] | Exploratory Data Analysis (EDA), visualization, and documentation |
| **Ishita Gabhane** | @[INSERT HANDLE] | Baseline modeling (Logistic Regression) and performance metrics |
| **Xiomara Serpa** | @[INSERT HANDLE] | Advanced modeling (Neural Networks) and hyperparameter tuning |
| **Chinyere Ugwuanyi** | @[INSERT HANDLE] | Project coordination, business context integration, and presentation |

---

## 🎯 **Project Highlights**

* **High-Performance Classification:** Achieved **98.33% accuracy** using a Random Forest model with TF-IDF features, successfully distinguishing between real and fake news articles.
* **Business-Centric Solution:** Developed a scalable content moderation tool to support Accenture's Trust & Safety goals, mitigating legal liability and reputational risk.
* **Bias Mitigation:** Identified and removed a critical source of data leakage (the "Reuters" tag) which appeared in 99.8% of real news, ensuring the model learned linguistic patterns rather than source shortcuts.
* **Robust Preprocessing:** Implemented a rigorous cleaning pipeline that removed over 5,000 duplicate texts and handled empty content to ensure data quality.

---

## 👩🏽‍💻 **Setup and Installation**

### **Repository Structure**
```text
├── data/                # Dataset files (excluded from repo via .gitignore)
├── notebooks/           # Jupyter notebooks for EDA and Modeling
├── src/                 # Python scripts for modular code
│   ├── preprocessing.py # Cleaning and tokenization functions
│   └── evaluation.py    # Metric calculation and plotting functions
├── images/              # Images used in this README
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```


\#\# 🎯 \*\*Project Highlights\*\*

\*\*Example:\*\*

\- Developed a machine learning model using \`\[model type/technique\]\` to address \`\[challenge project task\]\`.  
\- Achieved \`\[key metric or result\]\`, demonstrating \`\[value or impact\]\` for \`\[host company\]\`.  
\- Generated actionable insights to inform business decisions at \`\[host company or stakeholders\]\`.  
\- Implemented \`\[specific methodology\]\` to address industry constraints or expectations.

\---

\#\# 👩🏽‍💻 \*\*Setup and Installation\*\*

## 🚀 Installation Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/REPO_NAME.git
cd REPO_NAME
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
4. Run the Jupyter Notebook

Navigate to the notebooks/ directory
Open the main analysis notebook
Ensure the dataset files (True.csv and Fake.csv) are placed in the data/ directory
```
\---
## 🏗️ **Project Overview**

**Describe:**

- **Connection to the Break Through Tech AI Program**  
  This project was developed as part of the **Break Through Tech AI Program (AI Studio)**, where participants collaborate on industry-relevant machine learning challenges and apply AI techniques to real-world problems.

- **AI Studio Host Company, Objective, and Scope**  
  This project addresses a critical challenge within **Accenture’s Trust & Safety domain**.  
  The objective was to build a **binary classification model** capable of detecting **fake news** (fabricated stories) versus **real news** (factual articles) using **Natural Language Processing (NLP)** and **Machine Learning** techniques.

- **Real-World Significance and Impact**  
  In the digital age, misinformation can spread globally within minutes, making manual content review impossible at scale. Automated detection systems are essential to:
  - Safeguard brand trust and public institutions  
  - Mitigate financial and reputational risks for platforms and advertisers  
  - Enable scalable, real-time content moderation  

---

## 📊 **Data Exploration**

**You might consider describing the following (as applicable):**

- **Dataset Description**  
  We utilized a dataset containing approximately **45,000 news articles**, split into two CSV files:
  - **Real News (~21,000 articles):** Factual articles from reputable sources  
  - **Fake News (~23,000 articles):** Fabricated or misleading content  

  **Features included:**  
  - Title  
  - Body Text  
  - Subject  
  - Date  

- **Data Exploration and Preprocessing**  
  Data quality was a critical focus. Our preprocessing pipeline included:
  - **Noise Reduction:** Removal of HTML tags, URLs, and punctuation  
  - **Handling Missing Data:** Dropped **652 rows** with empty or significantly short text (<10 characters)  
  - **Deduplication:** Removed **5,402 duplicate entries** to prevent data leakage between training and testing sets  
  - **Bias Removal:**  
    The word *“Reuters”* appeared in **99.8%** of real news articles but only **1.3%** of fake news articles. This tag was removed to ensure the model learned linguistic patterns rather than relying on a source identifier.

- **EDA Insights**
  - **Text Length Distribution:** Fake news articles tended to be shorter on average compared to real news. This insight informed the creation of a **Text Length** metadata feature.  
    *(Note: Upload the histogram from Slide 19 here)*  
  - **Class Balance:** After preprocessing, the dataset remained well-balanced, reducing the risk of bias toward a majority class.

- **Challenges and Assumptions**
  - Assumed article text contained sufficient signals for classification  
  - Addressed dataset bias to avoid artificially inflated model performance  
  - Ensured preprocessing steps did not introduce data leakage  

**Potential visualizations to include:**
- Text length histogram  
- Class distribution chart  

---

## 🧠 **Model Development**

**You might consider describing the following (as applicable):**

- **Models Used**
  - **Baseline Model:** Logistic Regression (simple and interpretable)  
  - **Advanced Models:**  
    - Random Forest  
    - XGBoost (to capture non-linear relationships)  
    - Neural Networks (to capture complex semantic patterns)

- **Feature Selection and Hyperparameter Tuning**
  - **TF-IDF Vectorization:** Unigrams and bigrams  
  - **Metadata Features:** Text length, title length, sentiment scores  
  - Used `GridSearchCV` to tune Random Forest hyperparameters:
    - `n_estimators = 200`  
    - `criterion = 'entropy'`

- **Training Setup**
  - Data split into **training, validation, and test sets**  
  - Vectorizers fitted only on training data to prevent data leakage  
  - Models optimized for **Accuracy** and **Recall**, prioritizing the detection of fake news  

- **Code Highlights**
  - `preprocessing.py`: Custom regex logic to remove the *Reuters* source bias  
  - `modeling.ipynb`: Model training and hyperparameter tuning workflows  

---

## 📈 **Results & Key Findings**

**You might consider describing the following (as applicable):**

- **Performance Metrics**
  - Accuracy  
  - ROC-AUC  
  - Precision and Recall  

- **Model Performance Summary**

| Model | Accuracy | ROC-AUC | Key Observation |
|------|----------|---------|----------------|
| Random Forest (TF-IDF) | 98.33% | 99.71% | Best overall performance; robust to overfitting |
| XGBoost | 98.30% | 99.86% | Very competitive, slightly slower training |
| Logistic Regression | 97.98% | 99.71% | Simple model proved highly effective |
| Neural Network | 97.35% | 99.44% | Strong results but higher computational cost |

- **Key Insights**
  The **Random Forest with TF-IDF features** performed best, achieving the strongest balance of Precision and Recall—critical for content moderation use cases.

- **Fairness and Evaluation Insights**
  - Balanced dataset reduced class bias  
  - Bias removal improved generalization  
  - Very low false negatives observed, minimizing missed fake news cases  

**Potential visualizations to include:**
- Model comparison bar chart *(Slide 27)*  
- Confusion matrix for the best model *(Slide 24)*  

---

## 🚀 **Next Steps**

**You might consider addressing the following (as applicable):**

- **Limitations**
  - Tree-based models showed signs of overfitting (100% training accuracy)  
  - Model performance is dependent on historical news patterns  
  - Limited interpretability for non-technical stakeholders  

- **Future Improvements**
  - Further hyperparameter tuning for Neural Networks and TF-IDF settings  
  - Implement transformer-based models (BERT, RoBERTa) for deeper semantic understanding  
  - Explore ensembling Random Forest and XGBoost for improved performance  
  - Integrate explainability tools such as **SHAP** or **LIME** to support human moderation workflows  

---

## 📝 **License**

This project is licensed under the **MIT License**.  
See the `LICENSE` file for details.

---

## 🙏 **Acknowledgements**

Special thanks to our **Accenture Challenge Advisors**:
- Jenna Hunte  
- Tate Arevalo  
- Isabel Heard  

And the **Break Through Tech AI Program team** for their guidance and support throughout the semester.
