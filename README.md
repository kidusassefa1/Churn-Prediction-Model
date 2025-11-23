# Customer Churn Prediction using Neural Networks

This project builds a machine learning model to predict customer churn using a simple Artificial Neural Network (ANN). Churn refers to customers who cancel or leave a service. The goal of this project is to identify patterns that help determine which customers are likely to stop using the service.

### **Dataset**
The project uses the Telco Customer Churn dataset.  
Rows represent customers, and columns describe account details, billing, service subscriptions, and demographic features.

- 7,043 rows (customers)
- 21 columns (features)
- **Target column:** `Churn` (Yes/No)

Example attributes include:
- Contract type
- Payment method
- Online security / technical support
- Monthly and total charges
- Tenure (how long they stayed)

---

### **Project Structure**

| Step | Description |
|------|------------|
| **1. Data Exploration** | Loaded dataset, viewed rows, analyzed structure, plotted churn distribution. |
| **2. Data Preprocessing** | Cleaned missing values, removed ID column, encoded categorical columns, normalized features. |
| **3. Modeling (ANN)** | Built a neural network using TensorFlow/Keras with ReLU layers and sigmoid output. |
| **4. Evaluation** | Measured accuracy, confusion matrix, and classification report. |

---

### **Model Architecture**

```text
Input Layer: Number of features after preprocessing
Hidden Layer 1: Dense(16, activation='relu')
Hidden Layer 2: Dense(8, activation='relu')
Output Layer: Dense(1, activation='sigmoid')
Loss: binary_crossentropy
Optimizer: adam
