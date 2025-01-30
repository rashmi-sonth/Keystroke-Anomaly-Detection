# Enhanced Anomaly Detection in Keystroke Dynamics Authentication

This repository is part of the **CS266 - Topics in Information Security** course project titled **"Enhanced Anomaly Detection in Keystroke Dynamics Authentication"**. The project focuses on analyzing different methodologies for anomaly detection in keystroke dynamics authentication, leveraging advanced machine learning and deep learning models.

---

## File Structure

### **1. Dataset**
- **`demographics.csv`**:
  - Contains demographic information of participants.
  - Used to supplement analysis with demographic-based features.
  
- **`free-text.csv`**:
  - Contains raw keystroke dynamics data.
  - Includes timing features such as `DU.key1.key1`, `DD.key1.key2`, etc.
  - This dataset is critical for building and testing machine learning models.

- **Dataset Source**:
  - The dataset used in this project can be downloaded from [Zenodo](https://zenodo.org/records/7886743).

### **2. Notebook**
- **`models.ipynb`**:
  - The main Jupyter Notebook for training and evaluating models.
  - Implements machine learning and deep learning approaches (e.g., LSTM, CNN).
  - **Important**: Ensure the dataset paths (`free-text.csv` and `demographics.csv`) are correctly updated in this notebook based on your local environment.

### **3. Output**
- **`output.png`**:
  - Helps to evaluate the effectiveness of implemented techniques.

---

## Instructions

1. **Update Dataset Paths**:
   - The datasets are located in the `dataset` folder.
   - Ensure you update the dataset paths in the `models.ipynb` file wherever necessary:
     ```python
     data = pd.read_csv('dataset/free-text.csv')
     demographics = pd.read_csv('dataset/demographics.csv')
     ```

2. **Run the Notebook**:
   - Open `models.ipynb` in Jupyter Notebook or any compatible environment.
   - Execute the cells step-by-step to train and evaluate the models.

---

## Requirements

- Python 3.7+
- Libraries:
  - `tensorflow`
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `sklearn`
