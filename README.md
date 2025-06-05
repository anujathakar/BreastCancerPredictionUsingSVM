# BreastCancerPredictionUsingSVM
This project uses **Support Vector Machines (SVM)** to classify whether a tumor is **malignant** or **benign** based on the features provided in the **Breast Cancer Wisconsin dataset**. It serves as a beginner-friendly example of binary classification in machine learning using Scikit-learn.

## Dataset

We use the built-in `load_breast_cancer()` dataset from Scikit-learn. It includes:
- 569 samples
- 30 numerical features (e.g., radius, texture, area, smoothness)
- Binary labels:
  - `0` → Malignant (cancerous)
  - `1` → Benign (non-cancerous)

---

## 🛠Technologies Used

- Python 
- Jupyter Notebook 
- Scikit-learn
- Pandas
- Seaborn / Matplotlib for visualization

---

## How the Project Works

### 1. Load the dataset  
We use Scikit-learn’s built-in breast cancer dataset and convert it into a Pandas DataFrame for easier handling.

### 2. Split into training and testing sets  
We split the dataset (70% train, 30% test) using `train_test_split`.

### 3. Train the SVM model  
A linear kernel SVM (`SVC(kernel='linear')`) is trained on the training data.

### 4. Make predictions  
We predict on the test set and compare against true labels.

### 5. Evaluate model performance  
We use:
- **Accuracy Score**
- **Confusion Matrix**
- **Classification Report** (Precision, Recall, F1-score)

---

## Sample Output

```bash
Accuracy: 0.9649

Classification Report:
              precision    recall  f1-score   support

           0       0.96      0.94      0.95        64
           1       0.97      0.98      0.97       107

    accuracy                           0.96       171
   macro avg       0.96      0.96      0.96       171
weighted avg       0.96      0.96      0.96       171
