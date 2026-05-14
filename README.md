# part-1-neural-network-analysis
# Customer Churn Neural Network Analysis

## Project Objective

The objective of this project is to build a feed-forward neural network model to predict customer churn.

The target variable is `churn`, where:
- 1 means customer churned
- 0 means customer retained

---

## Dataset Understanding

The dataset contains customer-related information such as:

- Region
- Plan Type
- Contract Type
- Payment Method
- Tenure
- Monthly Charges
- Login Days
- Support Tickets
- Data Usage
- Satisfaction Score
- Discount Usage
- Referrals

The column `customer_id` was removed because it is only an identifier and not useful for prediction.

---

## Data Preprocessing

The preprocessing steps included:

- Handling missing values
- Encoding categorical variables
- Feature scaling using StandardScaler
- Train-test split

---

## Neural Network Architecture

The neural network contains:

- Input Layer
- Hidden Layer 1 with ReLU activation
- Hidden Layer 2 with ReLU activation
- Output Layer with Sigmoid activation

Optimizer used:
- Adam

Loss Function:
- Binary Crossentropy

Evaluation Metric:
- Accuracy

---

## Training and Evaluation

The model performance was evaluated using:

- Accuracy Score
- Loss
- Confusion Matrix
- Classification Report

---

## Hyperparameter Experiments

Three experiments were performed by changing:

- Number of hidden layers
- Number of neurons
- Learning rate
- Batch size
- Number of epochs

The results were stored in:

`results/model_comparison.csv`

---

## Final Reflection

### Role of Weights and Biases

Weights help the neural network learn the importance of each feature. Biases help improve model flexibility and shift activation functions.

### Why Activation Functions are Required

Activation functions introduce non-linearity into the neural network so that complex patterns can be learned.

### Effect of Learning Rate

A very high learning rate can make training unstable. A very low learning rate slows down training significantly.

### Underfitting and Overfitting

Underfitting happens when the model fails to learn patterns properly. Overfitting happens when the model memorizes training data but performs poorly on unseen data.

The validation graphs were used to analyze underfitting and overfitting.
