# DDos-Attack-classification
Welcome to the Hierarchical Machine Learning-Based DDoS Attack Detection System! This project allows you to detect and classify Distributed Denial of Service (DDoS) attacks in network traffic with high accuracy using advanced machine learning techniques.
The project combines feature selection, data preprocessing, and hyperparameter optimization to provide reliable detection of malicious network activities while minimizing false positives.

## Table of Contents:
- [Background](#background)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Results](#results)
- [Extension](#extension)

## Background:
With the digitization of vital service sectors including banking, insurance, and telecommunications, users increasingly depend on online services. This digital transformation has led to heightened cybersecurity concerns, especially regarding DDoS attacks that can disrupt services and compromise sensitive information.
DDoS attacks flood servers with numerous requests, overwhelming bandwidth and making services unavailable to legitimate users. This project addresses the critical need for effective detection systems by implementing advanced machine learning techniques to identify attack patterns in network traffic.

## Features:
->Hierarchical Machine Learning Framework: Combines multiple algorithms for enhanced classification accuracy.<br>
->Advanced Preprocessing: Utilizes min-max scaling and SMOTE techniques to handle class imbalance.<br>
->Feature Selection: Implements LASSO for optimal feature identification.<br>
->Hyperparameter Optimization: All algorithms are pre-trained with optimized parameters.<br>
->High Accuracy: Achieves 99.77% classification accuracy using LGBM algorithm.<br>
->Modular Design: Structured into distinct modules for preprocessing, feature selection, and optimization.<br>
->User Interface: Flask-based front end with user authentication for easy testing.<br>

## Installation:
1)Clone the repository:
```bash# 
git clone https://github.com/your-username/DDoS-detection-system.git
cd DDoS-detection-system
```
2)Create and activate virtual environment (optional but recommended)
```bash#
python -m venv venv
source venv/bin/activate
```
3)Install dependencies
```bash#
pip install -r requirements.txt
```

## Usage:
1)Navigate to the project directory:<br>
2)Open Anaconda Prompt<br>
3)Navigate to your project folder in Anaconda prompt<br>
```bash#
 cd path\to\your\DDoS\folder
```
4)Launch the Flask application:
```bash#
python app.py
```
5)Access the web interface:<br>
Copy the generated local host URL (typically http://127.0.0.1:5000/)<br>
Paste the URL into your web browser<br>
6)User authentication:<br>
For new users: Click on "Register" and create an account<br>
For existing users: Login with your credentials<br>
7)Making predictions:<br>
Enter the required network traffic parameters (packets, bytes, segments, etc.)<br>
8)Click the "Predict" button<br>
View the prediction results showing whether the traffic is benign or a DDoS attack.<br>

## Methodology:
1)Data Preprocessing:<br>
Min-max scaling for feature normalization<br>
SMOTE technique for handling class imbalance<br>
2)Feature Selection:<br>
LASSO method to identify the most relevant features<br>
3)Model Training:<br>
Multiple machine learning algorithms implemented<br>
Hyperparameter optimization for each algorithm<br>
Model saved as model.sav for deployment<br>
4)Ensemble Techniques:<br>
Voting Classifier implementation for improved accuracy<br>
5)Evaluation:<br>
Performance assessment using metrics including recall, precision, accuracy, and F1-score<br>

## Results:
The system evaluation shows that the LGBM algorithm provides the highest classification accuracy at 99.77%, outperforming other machine learning algorithms in the study. The ensemble approach with Voting Classifier further enhances the prediction accuracy.

![image](https://github.com/user-attachments/assets/6af74323-d978-4cd8-996e-2dc60ed73225)

## Extension:
The project has been extended with:<br>
1)Ensemble Techniques: Implementation of Voting Classifier to enhance prediction accuracy<br>
2)Flask-based Front End: User-friendly interface for system testing and interaction (app.py and templates/ directory)<br>
3)User Authentication: Enhanced security features to restrict access to authorized users only (signup.db)<br>
