Habitability of Exoplanets
Predicting and Ranking Potentially Life-Supporting Worlds using Machine Learning
🚀 Why this project?

When I started exploring astronomy datasets, I kept asking one simple question:

“Out of thousands of discovered exoplanets… which ones could actually support life?”

Instead of manually studying each planet, I wanted to build a data-driven system that could:

analyze planetary & stellar properties

learn patterns of habitability

predict probabilities

and automatically rank the most promising planets

This project is my attempt to combine Astronomy + Data Science + Machine Learning into one practical solution.

👨‍💻 About Me

Jeyabalan R
B.Tech – Artificial Intelligence & Machine Learning
St. Joseph’s College of Engineering, Chennai

Interested in:

Machine Learning

Data Analytics

Real-world AI applications

Research-driven engineering

🎯 What this system does

✔ Cleans messy astronomical datasets
✔ Engineers meaningful scientific features
✔ Handles class imbalance
✔ Trains multiple ML models
✔ Compares performances
✔ Selects the best model
✔ Ranks exoplanets by habitability probability

Final output → A prioritized list of potentially habitable planets

📂 Project Structure
Habitability-of-Exoplanets/
│
├── data/            Raw & processed datasets
├── notebooks/       EDA + experiments
├── src/             ML pipeline code
├── models/          Saved models
├── outputs/         Rankings & results
├── index.html       Visualization/dashboard
└── README.md

🧠 My Approach (Step-by-Step Journey)
1️⃣ Understanding the Data First

I explored multiple datasets:

NASA Exoplanet Archive

Kepler Mission data

PHL Habitability Catalog

Kaggle datasets

Reality check:

Missing values everywhere

Inconsistent units

Outliers

No direct habitability labels

So cleaning became the first major task.

2️⃣ Data Cleaning

I focused heavily on making the data reliable:

Median imputation for missing values

Outlier removal (IQR)

Unit normalization

One-hot encoding for categorical features

Goal → Trust the data before trusting the model

3️⃣ Feature Engineering (Most important part)

Instead of blindly feeding raw columns, I designed:

⭐ Habitability Score Index (HSI)

Combines:

radius

temperature

orbital parameters

⭐ Stellar Compatibility Index (SCI)

Captures:

star temperature

luminosity

metallicity

These features made the model more physics-aware rather than purely statistical.

4️⃣ Handling Class Imbalance

Very few planets are habitable → dataset is skewed.

Used:

SMOTE oversampling

Stratified sampling

This improved:

Recall

F1-score

Stability

5️⃣ Model Experiments

I trained multiple algorithms to understand behavior:

Model	Observation
Logistic Regression	Strong baseline
KNN	Weak
Naive Bayes	Moderate
SVM	Good separation
Random Forest	Very stable
XGBoost	⭐ Best overall
🏆 Final Model Choice
👉 XGBoost

Reasons:

Handles non-linear relationships well

Robust to noise

Better multi-class performance

Higher weighted F1-score

Better probability estimates for ranking

📊 Evaluation Metrics Used

Accuracy

Precision

Recall

F1-score

ROC-AUC

Confusion Matrix

Focus was more on:
✔ Recall (don’t miss habitable planets)
✔ F1-score (balanced performance)

🌍 Final Output

The system produces:

Habitability predictions

Probability scores

Ranked exoplanet list

So astronomers can focus on:
👉 Top candidates first

🛠 Tech Stack

Python

Pandas

NumPy

Scikit-learn

XGBoost

Matplotlib

Jupyter Notebook

Git & GitHub

💡 What I Learned

This project taught me:

Real-world data is messy

Feature engineering matters more than fancy models

Handling imbalance is critical

Pipelines improve reproducibility

Domain knowledge improves ML

Most importantly:
👉 Good preprocessing beats complex algorithms

🔮 Future Plans

Next improvements I want to try:

CNN/LSTM for time-series light curves

SHAP for explainability

FastAPI deployment

Interactive dashboard

Auto data updates via NASA APIs

📌 How to Run
git clone <repo>
cd Habitability-of-Exoplanets
pip install -r requirements.txt
jupyter notebook


Run notebooks step-by-step.

⭐ Final Note

This project reflects both:

my technical skills

and my learning journey

If you find it useful or interesting, feel free to ⭐ the repo or share feedback!

Thanks for visiting 🚀
