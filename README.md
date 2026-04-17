📌 Ensemble Techniques: Stacking, Bagging & Boosting
📖 Overview

Ensemble learning is a powerful machine learning approach where multiple models are combined to improve overall performance. Instead of relying on a single model, ensemble methods leverage the strengths of multiple models to achieve better accuracy, stability, and generalization.

This project demonstrates three major ensemble techniques:

Bagging (Bootstrap Aggregating)
Boosting
Stacking
⚙️ Tech Stack
Programming Language: Python
Libraries Used:
NumPy
Pandas
Scikit-learn
Matplotlib / Seaborn (for visualization)
Environment: Jupyter Notebook
🧠 Ensemble Techniques Explained
1️⃣ Bagging (Bootstrap Aggregating)

👉 Concept:
Bagging reduces variance by training multiple models on different subsets of the dataset (created using random sampling with replacement).

👉 Key Idea:
Train multiple independent models in parallel and combine their predictions.

👉 Example Algorithm:

Random Forest

👉 Workflow:

Create multiple bootstrap samples from dataset
Train a model on each sample
Aggregate predictions (average / majority voting)

👉 Advantages:

Reduces overfitting
Improves stability
Works well with high-variance models (like decision trees)
2️⃣ Boosting

👉 Concept:
Boosting focuses on reducing bias by training models sequentially, where each new model tries to correct the errors of the previous one.

👉 Key Idea:
“Learn from mistakes”

👉 Example Algorithms:

AdaBoost
Gradient Boosting
XGBoost

👉 Workflow:

Train first model
Identify errors
Increase importance (weights) of misclassified points
Train next model on updated data
Combine all models

👉 Advantages:

High accuracy
Handles complex patterns
Reduces bias
3️⃣ Stacking (Stacked Generalization)

👉 Concept:
Stacking combines multiple different models and uses another model (meta-model) to make the final prediction.

👉 Key Idea:
“Model on top of models”

👉 Workflow:

Train multiple base models (e.g., Decision Tree, SVM, KNN)
Use their predictions as input features
Train a meta-model (e.g., Logistic Regression)
Final prediction is made by meta-model
