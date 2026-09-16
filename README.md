# spam-email-classifier
An NLP spam detector using TF-IDF and Naive Bayes/SVM to classify SMS/email messages as spam or ham, achieving ~95–98% accuracy.
Spam Email Classifier 📧

An NLP-based classification model that detects whether a message (SMS/email) is spam or ham (not spam). Built as part of the AI Internship at Codec Technologies.

📌 Project Overview

This project applies Natural Language Processing (NLP) and classical machine learning to filter spam messages based on their text content. It compares two classification algorithms — Naive Bayes and Support Vector Machine (SVM) — to see which performs better.

🎯 Objective
Preprocess raw text data (cleaning, stopword removal)
Convert text into numerical features using TF-IDF
Train and compare Naive Bayes and SVM classifiers
Evaluate performance using accuracy, precision, recall, and confusion matrices
📂 Dataset
Name: SMS Spam Collection dataset
Size: ~5,500 labeled messages (ham or spam)
Format: Tab-separated text file (label + message)
Source: Fetched directly in the notebook from a public GitHub-hosted copy
🛠️ Tech Stack
Python 3
pandas, NumPy
NLTK (text preprocessing, stopwords)
scikit-learn (TF-IDF, Naive Bayes, SVM, evaluation metrics)
Matplotlib & Seaborn (visualization)
joblib (model persistence)
🧠 Approach
Text Cleaning: lowercase conversion, punctuation/number removal, stopword removal
Feature Extraction: TF-IDF vectorization (top 3,000 features)
Modeling: trained both Multinomial Naive Bayes and linear-kernel SVM
Evaluation: compared accuracy and confusion matrices side by side
Testing: ran predictions on custom example messages
🚀 How to Run
Open Spam_Email_Classifier.ipynb in Google Colab
Run all cells: Runtime → Run all
The notebook downloads the dataset automatically (requires internet access, available by default in Colab)
📊 Results
Both models achieve ~95–98% accuracy on the test set
SVM generally shows slightly better precision on spam detection
Confusion matrices and classification reports included in the notebook
Custom test messages correctly classified as spam/ham
📈 Possible Improvements
Try additional algorithms (Logistic Regression, Random Forest)
Use word embeddings (Word2Vec, GloVe) instead of TF-IDF
Address class imbalance more explicitly (spam is the minority class)
Build a simple web interface for live message classification
📁 Repository Structure
spam-email-classifier/
├── Spam_Email_Classifier.ipynb   # Main notebook
├── spam_classifier_model.pkl     # Saved trained model (SVM)
├── tfidf_vectorizer.pkl          # Saved TF-IDF vectorizer
└── README.md                     # Project documentation
🙋 Author

AI Intern, Codec Technologies

📄 License

This project is for educational purposes as part of an internship assignment.
