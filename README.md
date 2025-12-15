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

\#\# 🎯 \*\*Project Highlights\*\*

\*\*Example:\*\*

\- Developed a machine learning model using \`\[model type/technique\]\` to address \`\[challenge project task\]\`.  
\- Achieved \`\[key metric or result\]\`, demonstrating \`\[value or impact\]\` for \`\[host company\]\`.  
\- Generated actionable insights to inform business decisions at \`\[host company or stakeholders\]\`.  
\- Implemented \`\[specific methodology\]\` to address industry constraints or expectations.

\---

\#\# 👩🏽‍💻 \*\*Setup and Installation\*\*

\*\*Provide step-by-step instructions so someone else can run your code and reproduce your results. Depending on your setup, include:\*\*

\* How to clone the repository  
\* How to install dependencies  
\* How to set up the environment  
\* How to access the dataset(s)  
\* How to run the notebook or scripts

\---

\#\# 🏗️ \*\*Project Overview\*\*

\*\*Describe:\*\*

\- How this project is connected to the Break Through Tech AI Program  
\- Your AI Studio host company and the project objective and scope  
\- The real-world significance of the problem and the potential impact of your work

\---

\#\# 📊 \*\*Data Exploration\*\*

\*\*You might consider describing the following (as applicable):\*\*

\* The dataset(s) used: origin, format, size, type of data  
\* Data exploration and preprocessing approaches  
\* Insights from your Exploratory Data Analysis (EDA)  
\* Challenges and assumptions when working with the dataset(s)

\*\*Potential visualizations to include:\*\*

\* Plots, charts, heatmaps, feature visualizations, sample dataset images

\---

\#\# 🧠 \*\*Model Development\*\*

\*\*You might consider describing the following (as applicable):\*\*

\* Model(s) used (e.g., CNN with transfer learning, regression models)  
\* Feature selection and Hyperparameter tuning strategies  
\* Training setup (e.g., % of data for training/validation, evaluation metric, baseline performance)

\---

\#\# 📈 \*\*Results & Key Findings\*\*

\*\*You might consider describing the following (as applicable):\*\*

\* Performance metrics (e.g., Accuracy, F1 score, RMSE)  
\* How your model performed  
\* Insights from evaluating model fairness

\*\*Potential visualizations to include:\*\*

\* Confusion matrix, precision-recall curve, feature importance plot, prediction distribution, outputs from fairness or explainability tools

\---

\#\# 🚀 \*\*Next Steps\*\*

\*\*You might consider addressing the following (as applicable):\*\*

\* What are some of the limitations of your model?  
\* What would you do differently with more time/resources?  
\* What additional datasets or techniques would you explore?

\---

\#\# 📝 \*\*License\*\*

If applicable, indicate how your project can be used by others by specifying and linking to an open source license type (e.g., MIT, Apache 2.0). Make sure your Challenge Advisor approves of the selected license type.

\*\*Example:\*\*  
This project is licensed under the MIT License.

\---

\#\# 📄 \*\*References\*\* (Optional but encouraged)

Cite relevant papers, articles, or resources that supported your project.

\---

\#\# 🙏 \*\*Acknowledgements\*\* (Optional but encouraged)

Thank your Challenge Advisor, host company representatives, TA, and others who supported your project.

