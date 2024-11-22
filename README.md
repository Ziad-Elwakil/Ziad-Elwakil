1. Introduction
 This project focuses on the sentiment analysis of tweets using the Sentiment140 dataset. The
 objective is to classify the sentiment of tweets as either 'Positive' or 'Negative' using the DistilBERT
 model, a state-of-the-art sequence classification model. The project includes data loading,
 exploratory data analysis (EDA), model training, and the creation of a web application using
 Streamlit for user input sentiment predictions.
 2. Data Loading and Processing
 The Sentiment140 dataset containing 1.6 million tweets classified as 0 (Negative) or 4 (Positive) is
 downloaded from Kaggle. The dataset is loaded into a Pandas DataFrame, and the columns are
 renamed for easier handling. The target values are mapped to more readable formats (0 = Negative,
 1 = Positive). Data cleaning is performed to handle missing or incorrect dates. A new column,
 'text_length', is added to calculate the length of each tweet.
 3. Exploratory Data Analysis (EDA)
 Various visualizations are created to better understand the data, including:- Distribution of tweet lengths.- Sentiment distribution showing counts of positive and negative sentiments.- Boxplot of tweet lengths by sentiment.- Daily sentiment trends to show how sentiments change over time.
 4. Data Preparation for Modeling
 To achieve a balanced dataset, a sample of 100,000 tweets from both positive and negative
 categories is taken. The data is split into training and test sets using an 80-20 ratio, and the text
 data is tokenized using the DistilBERT tokenizer.
 5. Model Training
 The DistilBERT model is employed for text classification. The model is trained using the Hugging
 Face Transformers library with a Trainer interface. Important hyperparameters such as batch size,
number of epochs, warmup steps, and weight decay are configured to optimize performance.
 6. Model Evaluation
 After training, the model is evaluated using a classification report that provides various metrics such
 as accuracy, precision, recall, and F1-score, giving insights into the model's performance on the test
 data.
 7. Streamlit Application
 The project features a Streamlit interface allowing users to input text (tweets) and analyze their
 sentiments. The application also provides exploratory analyses, including sentiment distribution,
 tweet length distribution, and daily sentiment trends, all presented within an interactive environment.
 8. Conclusion
 The project successfully implements sentiment analysis using the DistilBERT model. The
 exploratory data analysis provides valuable insights into the dataset, while the modeling phase
 demonstrates the effectiveness of transformer-based models in classifying texts. Integrating the
 application with Streamlit enhances the interactivity of the project, allowing users to classify new
 tweets directly
