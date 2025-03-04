# ACSCE_NEUROCODESRS
AI Customer Sentiment Analysis Web Application:
Project Overview
This Sentiment Analysis Web Application is designed to analyze the sentiment of text data and classify it as Positive, Negative, or Neutral. It utilizes natural language processing (NLP) techniques to determine the sentiment conveyed in a given text input. The project is implemented using Python, with a primary focus on the use of TextBlob for sentiment analysis, alongside Flask for creating the web interface.

Key Features
Real-time Sentiment Prediction: The application processes user input and outputs the sentiment prediction instantly (Positive, Negative, or Neutral).
Flask Web Application: The user interface is built with Flask, which allows the user to interact with the sentiment analysis model easily.
CSV File Download: Users can download the results of the analysis in a CSV format.
Interactive Frontend: Users can input text, click the analyze button, and get immediate results displayed on the webpage.
Technologies Used
1. Python
The backend of the application is built using Python, a popular programming language widely used for data science, machine learning, and web development. Python provides all the necessary libraries for text processing and machine learning that make this project possible.

2. Flask
Flask is a micro web framework for Python. It is lightweight and easy to use, making it ideal for building simple web applications like this one. Flask handles user requests and serves the HTML interface to the users.

3. TextBlob
TextBlob is a Python library for processing textual data. It simplifies many natural language processing tasks, including sentiment analysis. TextBlob’s PatternAnalyzer is used in this project to analyze the sentiment of the given text. The analyzer classifies the sentiment into three categories:

Positive: If the text expresses positivity.
Negative: If the text expresses negativity.
Neutral: If the text neither expresses strong positive nor negative sentiment.
4. scikit-learn
For advanced text classification, scikit-learn provides powerful machine learning algorithms. It is used to build models that classify the sentiment of the text based on pre-trained data. In this project, Logistic Regression or SVM (Support Vector Machine) models can be used to enhance the analysis.

5. NLTK
NLTK (Natural Language Toolkit) is a library for working with human language data. It helps with text preprocessing, tokenization, and cleaning tasks, making it easier to prepare data for analysis. In this project, NLTK is used to handle and preprocess textual data before feeding it to the model.

6. pandas
pandas is used for data manipulation, especially when handling CSV files. The results of sentiment analysis can be stored and exported in CSV format for later use.

How the Application Works
Step 1: Text Input
The user opens the application in their web browser and is presented with a simple text box where they can input any text. This text can be anything, such as a tweet, a sentence, or a paragraph.

Step 2: Sentiment Prediction
When the user clicks the “Analyze” button, the text is passed to the backend where it is processed using TextBlob for sentiment analysis. The TextBlob library assigns a polarity score to the text and determines whether the sentiment is Positive, Negative, or Neutral.

Additionally, you may also use a pre-trained model (like Logistic Regression or SVM) from scikit-learn to improve the prediction accuracy based on historical data.

Step 3: Displaying Results
The application then displays the sentiment result on the webpage (e.g., "This is a Positive statement" or "This is a Negative statement"). The result is shown immediately, so the user knows the sentiment of their input.

Step 4: Downloading Results
The user can download the sentiment analysis result as a CSV file, which contains the input text and its corresponding sentiment. This feature allows users to save and later analyze the predictions.

Pre-trained Models
Sentiment Model: The pre-trained sentiment model, sentiment_model.joblib, is stored within the project directory. This model is used to make predictions for new input text.
TF-IDF Vectorizer: tfidf_vectorizer.joblib is used to convert text data into numerical format (vectorization) so it can be used by the machine learning models.
Working Flow of the Application
User Interface: The Flask app serves an HTML page with a form where users can enter text.
Text Processing: When the user submits the text, Flask routes the request to the backend where the text is processed using TextBlob.
Sentiment Analysis: The sentiment analysis is performed using TextBlob (or another model trained with scikit-learn), which outputs the sentiment (positive, negative, neutral).
Displaying Results: The sentiment result is displayed to the user on the webpage.
CSV Export: Users can download a CSV file containing the analyzed sentiment data.
Error Handling
If the CSV file for input text has missing data or cannot be read, an error message is displayed on the webpage.
The application also checks for any missing dependencies, such as TextBlob corpora and NLTK data files, and instructs users to download them if necessary.
Conclusion
This Sentiment Analysis Web Application serves as an efficient way to analyze the sentiment of text inputs. It is designed to be easy to use and can be extended for other NLP tasks. The use of Flask makes it lightweight and easy to deploy, while libraries like TextBlob and scikit-learn ensure the accuracy of sentiment predictions.

