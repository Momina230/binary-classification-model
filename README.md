# binary-classification-model
#  Student Depression Classification using Neural Networks

This project builds a **binary classification model** to detect student depression based on survey responses. It includes:

- A **custom neural network implemented from scratch using NumPy**, including backpropagation and Adam optimization.
- A benchmark model using **Scikit-learn's `MLPClassifier`**.
- Feature preprocessing using **Pandas** and **OneHotEncoding**.
- Accuracy evaluation and performance comparison between custom and library-based models.

---

##  Dataset

The dataset used is titled:  
**`Student Depression Dataset.csv`**

**Columns include:**

- Demographics (e.g., Gender, Age, City, Profession)
- Academic and Work Pressure
- Mental health indicators (e.g., Suicidal Thoughts, Depression)
- Lifestyle variables (e.g., Sleep, Diet)
- **Target**: `Depression` (Yes/No)

>  *Note: File is read from `/content/student-depression-dataset/Student Depression Dataset.csv` for Google Colab compatibility. Adjust path accordingly for local execution.*

---

##  Models Implemented

### 1. **Custom Neural Network (NumPy)**

- Fully connected feedforward network
- 1 hidden layer with 64 neurons
- Activation: Sigmoid
- Optimizer: Adam
- Manual implementation of:
  - Forward pass
  - Backward pass
  - Loss: Binary Cross-Entropy
- Accuracy printed for training and test sets

### 2. **Scikit-learn MLPClassifier**

- Hidden layer: 64 neurons
- Activation: Logistic (sigmoid)
- Optimizer: Adam
- Trained for 300 epochs
- Performance compared against custom NN

---

## 📊 Results

| Model Type         | Train Accuracy | Test Accuracy |
|--------------------|----------------|----------------|
| Custom NumPy NN    | ~0.95 (varies) | ~0.88–0.91     |
| Scikit-learn MLP   | ~0.94          | ~0.89          |

> Accuracy may vary based on dataset quality, preprocessing, and class balance.

---

##  Key Libraries Used

- `NumPy`
- `Pandas`
- `Scikit-learn` (for `MLPClassifier`, `OneHotEncoder`, `train_test_split`)
- `Google Colab` (optional)

---

##  How to Run

1. Clone the repository or copy the script to your workspace.
2. Place your CSV file in the correct path (or modify the `read_csv` path).
3. Install required libraries (if needed):

```bash
pip install numpy pandas scikit-learn
