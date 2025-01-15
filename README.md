# Predicting Job Eligibility of Salesman Applicants Using Deep Neural Networks

This repository contains a project aimed at predicting job eligibility for salesman applicants using a **Deep Neural Network (DNN)**. The dataset used includes interview responses and various metrics such as confidence, structured thinking, and fluency. The project showcases data preprocessing, feature reduction, model training, and deployment.

## Features
- **Dataset:** Kaggle dataset containing applicant data.
- **Deep Neural Network:** Predicts applicant eligibility with a test accuracy of **79.5%**.
- **Feature Reduction:** Dimensionality reduction from 52 features to 18 using JMAF software.
- **Frontend Interface:** Predicts applicant eligibility based on input features (to be added).

## Project Workflow

### 1. Data Preprocessing
- Handle missing values (numerical columns filled with medians).
- Encode categorical data using label encoding.
- Scale numerical data with StandardScaler.
- Apply feature reduction using JMAF software, reducing features from 52 to 18.

### 2. Deep Neural Network Architecture
- **Input Layer:** 18 neurons (one for each feature).
- **Hidden Layers:**
  - Layer 1: 128 neurons, ReLU activation, 30% dropout.
  - Layer 2: 64 neurons, ReLU activation, 30% dropout.
  - Layer 3: 32 neurons, ReLU activation.
- **Output Layer:** 1 neuron, Sigmoid activation (binary classification).

### 3. Model Configuration
- **Optimizer:** Adam
- **Loss Function:** Binary Cross-Entropy
- **Learning Rate:** 0.001
- **Epochs:** 50
- **Batch Size:** 16

### 4. Performance Metrics
- **Accuracy:** 79.5% on test data.
- **Confusion Matrix:** Evaluates model predictions.
- **Precision, Recall, F1-Score:** Additional evaluation metrics.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/job-eligibility-dnn.git
   cd job-eligibility-dnn
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the script:
   ```bash
   python main.py
   ```

## Files
- **main.py**: Main script for running the model.
- **data.csv**: Dataset file.
- **preprocessing.py**: Data cleaning and feature reduction.
- **model.py**: Deep Neural Network implementation.
- **requirements.txt**: Required Python libraries.

## Results
- **Model Accuracy:** 79.5%
- **Loss Plot:** Indicates training and testing loss over epochs.
- **Accuracy Plot:** Visualizes accuracy trends during training.

## Expected Outcomes
- A scalable **frontend interface** for job eligibility prediction.
- Improved recruitment accuracy and efficiency.

## Future Improvements
- Experiment with **hyperparameter tuning** for better accuracy.
- Add a **real-time prediction API**.
- Extend the model for multi-class classification tasks.

## References
1. [TensorFlow Documentation](https://www.tensorflow.org/)
2. [Kaggle Dataset](https://www.kaggle.com/)
3. Research papers on AI in recruitment.
4. Deep Learning with Python by François Chollet.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

Feel free to contribute or raise issues for improvements!
