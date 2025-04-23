# 📞 Telecom Customer Churn Prediction & Data Visualization

This project focuses on **predicting customer churn** in the telecom industry using various machine learning models and includes **data visualization** for better understanding of customer behavior. The dataset used is publicly available and sourced from [YBI Foundation](https://github.com/YBIFoundation/Dataset/raw/main/TelecomCustomerChurn.csv).

---

## 📂 Dataset

- **Source**: [TelecomCustomerChurn.csv](https://github.com/YBIFoundation/Dataset/raw/main/TelecomCustomerChurn.csv)
- **Content**: Contains features related to customer demographics, account information, and usage metrics.
- **Target**: `Churn` (whether the customer has left the service or not)

---

## 🧠 Machine Learning Models Used
python
models = {
    "Logistic Regression": LogisticRegression(max_iter=1000),
    "Random Forest": RandomForestClassifier(),
    "Gradient Boosting": GradientBoostingClassifier(),
    "XGBoost": XGBClassifier(use_label_encoder=False, eval_metric='logloss'),
    "LightGBM": LGBMClassifier(),
    "K-Nearest Neighbors": KNeighborsClassifier(),
    "SVC": SVC(),
    "MLP Classifier": MLPClassifier(max_iter=500)
}
### ✅ Evaluation Techniques

- **Standard Validation Split**
- **K-Fold Cross Validation**

---

## 📊 Model Accuracy Scores (Mean Comparison)

| Model                | Without K-Fold | With K-Fold |
|---------------------|----------------|-------------|
| Logistic Regression | 0.765          | 0.765       |
| Random Forest       | 0.876          | 0.875       |
| Gradient Boosting   | 0.782          | 0.784       |
| XGBoost             | 0.845          | 0.842       |
| LightGBM            | 0.822          | 0.815       |
| KNN                 | 0.749          | 0.750       |
| SVC                 | 0.777          | 0.775       |
| MLP Classifier      | 0.810          | 0.804       |

> _Note: Means are approximated from model performance arrays._

---

## 📈 Data Visualization

This project also includes a variety of visualizations to explore trends and patterns in the dataset, such as:

- Distribution of churned vs. retained customers
- Correlation heatmaps
- Service usage statistics
- Demographic distributions (gender, senior citizens, etc.)
- Boxplots, histograms, and count plots

These visualizations were created using:
- `Matplotlib`
- `Seaborn`
- `Pandas`

---

## 🚀 Getting Started

1. Clone the repo:
bash
   git clone https://github.com/Meanhor/Telecom-Customer-Churn.git
   cd telecom-customer-churn
   
2. Install required packages:
bash
   pip install -r requirements.txt
   
3. Run the notebook or script:
bash
   jupyter notebook Churn_Prediction.ipynb
   
---

## 📁 Project Structure

📦 telecom-customer-churn
├── 📊 Churn_Prediction.ipynb        # Main notebook
├── 📁 data                          # Dataset folder
├── 📈 tele-churn-visualize.ipynb               # Folder containing graphs and plots
├── 📄 requirements.txt              # Required Python packages
└── README.md                        # This file
---

## 🧑‍💻 Author

- **Kea Meanhor**
- [LinkedIn](https://www.linkedin.com/in/kea-meanhor) | [Portfolio](https://meanhor-portfolio.vercel.app/home)

---

## 📜 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

- Dataset provided by [YBI Foundation](https://github.com/YBIFoundation)


---

Let me know if you want me to add badges (like Python version, license, notebook status) or generate a requirements.txt for your repo!