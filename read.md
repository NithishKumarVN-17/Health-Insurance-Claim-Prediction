# Automatic Ticket Classification using NLP and ML

For a financial company, customer complaints are crucial as they provide insights into the shortcomings of their products and services. Resolving complaints efficiently and on time can reduce customer dissatisfaction and strengthen their loyalty. Additionally, it allows companies to continuously improve their services to attract more customers.

This project aims to automate the customer support ticket system of a financial company using Natural Language Processing (NLP) and Machine Learning (ML) techniques. The goal is to accurately identify and categorize support tickets based on their content and assign them to the relevant team for swift resolution.

## Table of Contents
- [Problem Statement](#problem-statement)
- [Solution](#solution)
- [Features](#features)
- [Classification Categories](#classification-categories)
- [Model Evaluation Metrics](#model-evaluation-metrics)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Logging](#logging)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Conclusion](#conclusion)

## Problem Statement

As a financial company with many products and services such as credit cards, banking, and mortgages/loans, the firm receives numerous customer complaints. These complaints, in the form of unstructured text data, need to be evaluated and assigned to the relevant department. Traditionally, this task requires multiple support employees, which can be time-consuming and inefficient as the company grows.

## Solution

To automate the customer support ticket system, we use NLP techniques to process and analyze the text data. We apply ML algorithms to classify support tickets based on their content and assign them to the relevant team. The ML component of this project utilizes powerful algorithms that predict the ticket's category based on the content of the ticket, achieving high accuracy rates.

## Features

- Flask-based web interface for submitting support tickets
- Text processing pipeline including cleaning, lemmatization, and POS tagging
- Word2Vec-based vectorization of processed text
- Machine learning model for ticket classification
- Logging system for tracking application behavior and predictions
- Automatic ticket classification using NLP and ML algorithms
- Accurate identification and categorization of support tickets
- Efficient assignment of support tickets to the relevant team for swift resolution

## Classification Categories

The system classifies support tickets into the following categories:

1. Bank account services
2. Credit Card/Prepaid Card
3. Mortgages/Loans
4. Theft/Dispute reporting
5. Others

## Model Evaluation Metrics

The following table summarizes the evaluation metrics for each of the models used in this project:

| Model                   | Accuracy | Precision | Recall | F1 Score | ROC AUC Score |
|-------------------------|----------|-----------|--------|----------|---------------|
| Logistic Regression     | 0.91     | 0.91      | 0.91   | 0.91     | 0.99          |
| DecisionTreeClassifier  | 0.78     | 0.78      | 0.78   | 0.78     | 0.86          |
| RandomForestClassifier  | 0.82     | 0.83      | 0.82   | 0.81     | 0.97          |
| MultinomialNB           | 0.71     | 0.74      | 0.71   | 0.67     | 0.94          |
| XGBClassifier           | 0.91     | 0.91      | 0.91   | 0.91     | 0.99          |

Based on these metrics, the Logistic Regression and XGBClassifier models performed the best, with high accuracy, precision, recall, F1 score, and ROC AUC score.

## Technologies

- Python
- Natural Language Processing (NLTK, spaCy)
- Machine Learning (scikit-learn, XGBoost)
- Flask
- Word2Vec

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/support-ticket-classification.git
   ```

2. Navigate to the project directory:
   ```
   cd support-ticket-classification
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Ensure you have the pre-trained models in the `Models` directory:
   - `word2vec_model.pkl`
   - `support_classification_model.pkl`

## Usage

1. Run the Flask application:
   ```
   python app.py
   ```

2. Open a web browser and navigate to `http://localhost:5000`

3. Enter the text of a support ticket in the input field and submit for classification.

4. View the predicted category for the support ticket.

## Project Structure

```
support-ticket-classification/
│
├── app.py                 # Main Flask application
├── Models/
│   ├── word2vec_model.pkl        # Pre-trained Word2Vec model
│   └── support_classification_model.pkl  # Pre-trained classification model
├── templates/
│   └── index.html         # HTML template for the web interface
├── logs/
│   └── app.log            # Application logs
└── README.md              # This file
```

## Logging

The application uses a rotating file handler for logging. Logs are stored in the `logs` directory, with the main log file named `app.log`. The logger is configured to create new log files when the current one reaches 10KB, keeping up to 10 backup files.

## Contributing

Contributions to improve the classification model, expand the categories, or enhance the web interface are welcome. Please feel free to submit a pull request or open an issue to discuss potential changes.

## License

[Insert your chosen license here, e.g., MIT, GPL, etc.]

## Contact

[Your Name] - [your.email@example.com]

Project Link: [https://github.com/yourusername/support-ticket-classification](https://github.com/yourusername/support-ticket-classification)

## Conclusion

"Automatic Ticket Classification using NLP and ML" is a valuable resource for any financial organization seeking to streamline their support ticket classification and resolution process. The automation of the customer support ticket system using NLP and ML techniques allows companies to efficiently identify and categorize support tickets, assign them to the relevant team for swift resolution, and continuously improve their products and services. This project demonstrates high accuracy in classifying tickets into specific categories relevant to financial services, enabling faster response times and improved customer satisfaction.
