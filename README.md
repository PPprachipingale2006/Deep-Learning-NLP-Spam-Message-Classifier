# Deep Learning NLP Spam Message Classifier

## Project Overview

The Deep Learning NLP Spam Message Classifier is a machine learning project that uses Natural Language Processing (NLP) and a deep learning neural network to classify SMS messages as Spam or Ham (legitimate messages).

The project is developed using Python, TensorFlow, and Keras. It demonstrates text preprocessing, tokenization, neural network training, model evaluation, and prediction on unseen messages.

## Objectives

- Build a deep learning model for SMS spam detection.
- Preprocess and tokenize text messages using NLP techniques.
- Train and validate a neural network using TensorFlow and Keras.
- Evaluate model performance using accuracy, loss, and classification metrics.
- Predict whether new messages are spam or legitimate.
- Save the trained model and evaluation results.

## Technologies Used

- Python
- Jupyter Notebook
- TensorFlow and Keras
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn

## Dataset

The project uses the SMS Spam Collection dataset from the UCI Machine Learning Repository.

Dataset source: https://archive.ics.uci.edu/dataset/228/sms+spam+collection

The dataset contains SMS messages labeled as:

- Ham: Legitimate messages, represented by 0.
- Spam: Unwanted or promotional messages, represented by 1.

The dataset is divided into 80% training data and 20% testing data.

## Project Structure

```text
NLP-Spam-Message-Classifier/
│
├── spam_classifier.ipynb
├── README.md
├── requirements.txt
│
├── spam_dataset/
│   └── SMSSpamCollection
│
└── outputs/
    ├── training_curves.png
    ├── confusion_matrix.png
    ├── classification_report.txt
    ├── sample_predictions.csv
    └── spam_classifier.keras
```

## Implementation Steps

### 1. Data Loading

Loaded the SMS Spam Collection dataset using Pandas and examined its structure and class distribution.

### 2. Text Preprocessing

Cleaned the text by converting messages to lowercase, removing unnecessary characters, and eliminating extra spaces.

### 3. Label Encoding

Converted the message labels into numerical values:

- Ham = 0
- Spam = 1

### 4. Data Splitting

Split the dataset into training and testing sets using an 80:20 ratio.

### 5. Tokenization and Vectorization

Used the Keras Tokenizer to convert words into numerical sequences. Applied padding to ensure that all messages have a fixed sequence length.

### 6. Deep Learning Model Development

Built a neural network using an embedding layer, dense layers, batch normalization, and dropout.

The model uses the Adam optimizer and binary cross-entropy loss function.

### 7. Model Training

Trained the neural network using training data and monitored its performance on validation data. Early stopping was used to prevent unnecessary training.

### 8. Model Evaluation

Evaluated the model using test accuracy, test loss, a confusion matrix, and a classification report containing precision, recall, and F1-score.

### 9. Prediction on New Messages

Tested the trained model on unseen SMS messages and generated predicted classes with confidence scores.

### 10. Model Saving

Saved the trained model in Keras format and exported the evaluation results and prediction outputs.

## Output Files

| File | Description |
|---|---|
| `training_curves.png` | Training and validation accuracy and loss graphs |
| `confusion_matrix.png` | Visualization of correct and incorrect classifications |
| `classification_report.txt` | Precision, recall, F1-score, and support |
| `sample_predictions.csv` | Predictions and confidence scores for sample messages |
| `spam_classifier.keras` | Saved trained neural network |

## Installation and Execution

### Step 1: Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/NLP-Spam-Message-Classifier.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### Step 2: Navigate to the project folder

```bash
cd NLP-Spam-Message-Classifier
```

### Step 3: Install the required libraries

```bash
pip install -r requirements.txt
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

Open `spam_classifier.ipynb` and run the notebook cells in order.

## Conclusion

The Deep Learning NLP Spam Message Classifier demonstrates the application of Natural Language Processing and neural networks to automated SMS spam detection. The model learns from labeled messages and predicts whether new messages are spam or legitimate.

The project includes data preprocessing, tokenization, model training, evaluation, and sample predictions. The trained model and evaluation results are saved for future use.

## Future Enhancements

- Improve model performance using advanced NLP architectures such as LSTM or Transformers.
- Deploy the model as a web application using Flask or Streamlit.
- Extend the classifier to support email spam detection.
- Test the model on larger and more diverse datasets.

## Author

Prachi Pingale

Deep Learning / NLP Project

