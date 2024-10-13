## Plagiarism Detection App
- Plagiarism detection is a crucial task in various domains, including academia, content creation, and software development. This application leverages natural language processing (NLP) techniques and machine learning to determine whether two input sentences exhibit plagiarism. By analyzing linguistic features and token similarities, the model provides a binary classification indicating the presence or absence of plagiarism.

# Features
- User-Friendly Interface: Simple and intuitive UI built with Streamlit.
- Text Preprocessing: Comprehensive preprocessing including decontraction, punctuation removal, and normalization.
- Feature Engineering: Extracts multiple linguistic and token-based features to enhance model performance.
- Plagiarism Prediction: Utilizes a pre-trained classifier to predict plagiarism based on input sentences.
- Additional Feature: Incorporates custom features derived from dataset observations to improve accuracy.

# Additional Feature
While developing this application, an additional feature was incorporated by closely analyzing the MIT PLAGAIRISM DETECTION DATASET(https://www.kaggle.com/datasets/ruvelpereira/mit-plagairism-detection-dataset?resource=download) and understanding the nuances of plagiarism detection. Specifically, the application includes token-based similarity metrics such as common word count, stop word intersections, and token position checks (e.g., first and last words matching). This feature was observed to significantly contribute to distinguishing plagiarized content from original content, thereby enhancing the model's predictive capabilities.

# Feature Engineering
Extracted a combination of basic and advanced features:

- Basic Features: Length of sentences, number of words, common word count, and total unique words.
- Token Features: Similarity ratios based on common words, stop words, token positions, etc.
- Length Features: Differences in sentence lengths and longest common substring ratios.

# Model Training
- Vectorization: Used a pre-trained vectorizer to convert text data into numerical format.
- Classifier: Employed Random forest classifier trained on the extracted features to predict plagiarism.

# Integration and Deployment
- Streamlit Interface: Developed an interactive web interface for users to input sentences and receive plagiarism predictions.
- The pre-trained model was deployed on Hugging Face's model hub, allowing for easy access and sharing.

# Installation
- Clone the Repository
```
git clone https://github.com/Rittik2002/plagiarism_detection_NLP.git
cd plagiarism_detection_NLP
```
- Install Dependencies
```
pip install -r requirements.txt
```

