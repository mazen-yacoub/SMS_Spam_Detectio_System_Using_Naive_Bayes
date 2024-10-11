# SMS Spam Detection System Using Naive Bayes
<div style="text-align: center;">
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTtKu2gKpAnqt0M5GVnE8g34SDfbh8wXnxQIQ&s" alt="My Image">
</div>

## Project Overview

The primary objective of this project was to classify SMS messages as either 'Spam' or 'Not Spam' utilizing the SMS Spam Collection dataset sourced from the UCI Machine Learning Repository. This classification task leverages the Naive Bayes theorem, a well-established probabilistic inference algorithm.

## Introduction to the Naive Bayes Theorem

Bayes' theorem, formulated by Reverend Thomas Bayes, remains one of the foundational algorithms in probabilistic inference. While originally applied to philosophical inquiries, it has found extensive use in various practical applications, including spam detection.

To illustrate the theorem, consider a scenario involving a Secret Service agent responsible for the safety of a Democratic presidential nominee during a public campaign event. In this context, the agent assesses potential threats based on specific features, such as age, gender, and observable behaviors like carrying a bag or appearing nervous. If an individual's characteristics raise sufficient suspicion, they may be identified as a potential threat and removed from the area.

Bayes' theorem computes the probability of an event (e.g., an individual being a threat) based on the probabilities of associated events (such as age, gender, and nervousness). A crucial element of this theorem is the assumption of feature independence. For example, a nervous child may pose a lower risk than a nervous adult. By analyzing both age and nervousness, we can minimize false positives, leading to a more accurate identification of non-threatening individuals.

The "Naive" aspect of the theorem refers to the presumption that all features are independent of each other. While this assumption simplifies calculations, it may not always reflect real-world scenarios, potentially influencing outcomes.

In summary, Bayes' theorem estimates the probability of a specific event (e.g., a message being classified as spam) by evaluating the joint probabilities of relevant features (such as the presence of particular words). We will delve into the specifics of Bayes' theorem later in this document, but first, let us review the dataset utilized in this project.

## Key Steps in the Project

### 1. Understanding the Dataset
- The dataset comprises 5,574 SMS messages, with each message labeled as either 'ham' (not spam) or 'spam'.

### 2. Data Preprocessing
- Converted the labels into binary values: 0 for 'ham' and 1 for 'spam'. This conversion is crucial for computational efficiency in machine learning.

### 3. Bag of Words (BoW)
- Implemented the Bag of Words model using `CountVectorizer` to transform SMS text into numerical data. This transformation is essential for enabling machine learning algorithms to process textual data.

### 4. Training and Testing Sets
- Divided the dataset into training and testing sets to evaluate the model's generalization capabilities on new data.

### 5. Naive Bayes Implementation
- Trained a Multinomial Naive Bayes classifier, which is particularly effective for text classification tasks.

### 6. Model Evaluation
- Evaluated the model using various metrics:
  - **Accuracy:** 0.98
  - **Precision:** 0.97
  - **Recall:** 0.94
  - **F1 Score:** 0.96

These metrics indicate that the model performs exceptionally well, especially in terms of precision and recall, which are critical for effective spam detection.

### 7. Prediction Function
- Developed a function to predict whether a new SMS message is spam or ham. Here are a couple of examples:
  - "Congratulations! You have won a free iPhone!" - **Prediction:** Spam
  - "Hey, are we still on for lunch tomorrow?" - **Prediction:** Ham

## Conclusion

This project has significantly enhanced my understanding of machine learning, natural language processing, and model evaluation metrics. I am eager to explore more complex models and datasets in future endeavors!
