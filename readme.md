# Employee Attrition & Department Prediction

This project leverages a multi-output neural network to predict both the **Department** an employee belongs to and whether they are likely to **leave the company (Attrition)**, based on various HR-related features.

## 📁 Project Structure

- `attrition.ipynb` – Main notebook containing data preprocessing, model building, training, and evaluation.
- `data` – https://static.bc-edx.com/ai/ail-v-1-0/m19/lms/datasets/attrition.csv
- `README.md` – Project overview and instructions.

## 🧠 Model Overview

This neural network performs **multi-output classification**:

- **Output 1**: Department (multiclass classification using `softmax`)
- **Output 2**: Attrition (binary classification using `sigmoid`)

### Key Components:
- TensorFlow/Keras for model implementation
- Categorical and binary crossentropy losses
- Accuracy metrics for both outputs
- EarlyStopping and validation split used during training

## 🔍 Evaluation

Each output is evaluated separately:
- Department Accuracy
- Attrition Accuracy

Custom metrics such as F1-score, precision, or recall may be used for deeper analysis, especially for the Attrition prediction.

## 🛠️ How to Run

1. Clone the repo:
   ```bash
   git clone <repo-url>
   cd <repo-folder>
2. python -m venv .venv
3. source .venv/bin/activate   # On Windows: .venv\Scripts\activate
3. pip install -r requirements.txt
4. jupyter notebook attrition.ipynb '''

### Sample Output Metrics
Department Accuracy: 0.87  
Attrition Accuracy: 0.71
