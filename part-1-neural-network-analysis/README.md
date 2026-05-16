**Customer Churn Prediction using Neural Networks**

This project implements a deep learning solution to predict customer churn. It follows a structured machine learning pipeline, from exploratory data analysis and preprocessing to building, evaluating, and fine-tuning a Neural Network model using TensorFlow and Keras.



**Project Overview**

The project is created using google Collab due to versioning issues encountered in VS code and Kernels related to Tensorflow were not getting installed. However, the project created on collab here uses the "customer\_churn\_nn.csv" dataset, which contains:

Features: Customer demographics, account information, and usage patterns (e.g., tenure, monthly charges, support tickets).

Target: "churn" (0 = No, 1 = Yes).



**Key Tasks \& Workflow**

1\. Dataset Understanding

Loaded the dataset and inspected its shape, data types, and missing values. Also, performed statistical summaries and visualized the distribution of the target variable.



2\. Data Preprocessing

Handling Missing Values: Used median imputation for numerical features and mode imputation for categorical features.

Scaled numerical features using "StandardScaler"

Encoded categorical features using "OneHotEncoder"

Divided the dataset into training (80%) and testing (20%) sets with stratification to maintain class proportions.



3\. Neural Network Model Building

Constructed a "Sequential" model using TensorFlow.



4\. Training and Evaluation

Trained the model for 20 epochs with a batch size of 32.

Visualizations: Generated plots for Training vs. Validation Accuracy and Loss.

Evaluated performance using a Confusion Matrix



5\. Hyperparameter Experimentation

Conducted experiments to optimize model performance by varying:

Network Depth: Added more hidden layers.

Learning Rate: Adjusted the Adam optimizer's learning rate.

Batch Size: Tested larger batch sizes (e.g., 64).



**Requirements**

To run this notebook, you need the following Python libraries:

"pandas", "numpy", "matplotlib", "seaborn", "scikit-learn" and "TensorFlow"



**How to Use**

Ensure `customer\_churn\_nn.csv` is in the same directory as the notebook.



