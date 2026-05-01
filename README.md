Linear Regression from Scratch 📈
A pure Python implementation of Linear Regression using gradient descent, built without any machine learning libraries. This project demonstrates a deep understanding of the math and mechanics behind one of the most fundamental ML algorithms.

🔍 Overview
This notebook implements Linear Regression entirely from scratch using only NumPy, Pandas, and Matplotlib — no scikit-learn, no shortcuts. The model is trained on a salary dataset to predict salary based on years of experience.

📂 Dataset
Salary Dataset (Salary_dataset.csv)
FeatureDescriptionYearsExperienceNumber of years of professional experienceSalaryAnnual salary (target variable)

Samples: 30
Task: Regression (predicting a continuous value)


⚙️ How It Works
1. Hypothesis Function
The model predicts salary using a linear equation:
ŷ = θ·x + c
where θ is the slope and c is the intercept.
2. Cost Function (Mean Squared Error)
J(θ, c) = (1 / 2m) · Σ (ŷᵢ - yᵢ)²
3. Gradient Descent
θ = θ - α · (1/m) · Σ xᵢ · (ŷᵢ - yᵢ)
c = c - α · (1/m) · Σ (ŷᵢ - yᵢ)
where α is the learning rate.

🛠️ Implementation Details
ParameterValueLearning Rate (α)0.001Epochs100Initial θ0Initial c0

📊 Results
After training:

Slope (θ): ~12482.56
Intercept (c): ~2309.29
Final MSE: ~70,176,339

The loss curve confirms successful convergence of gradient descent over 100 epochs.

📁 Project Structure
├── Salary_dataset.csv       # Training data
├── linear_regression.ipynb  # Main notebook
└── README.md

🚀 Getting Started
Prerequisites
bashpip install numpy pandas matplotlib
Run the Notebook
bashjupyter notebook linear_regression.ipynb

📈 Visualizations
The notebook includes three plots:

Scatter plot of the raw data (YearsExperience vs Salary)
Regression line fitted on the data after training
Loss landscape — MSE vs Slope and MSE vs Intercept showing gradient descent convergence


🧠 Key Concepts Demonstrated

Manual implementation of the MSE cost function
Gradient descent optimization from scratch
Understanding of partial derivatives for multi-parameter update
Loss curve tracking across epochs
Visualization of the loss landscape


🔧 Built With

Python 3.x
NumPy
Pandas
Matplotlib


👤 Author
Mohammad Awez Haider
B.Tech CSE (AI/ML) — C.V. Raman Global University
GitHub: @Hwk-Awez
