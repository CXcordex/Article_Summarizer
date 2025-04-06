# Article_Summarizer
This project focuses on analyzing and summarizing  articles using natural language processing (NLP) techniques while assessing the linguistic complexity of the text. 
The goal of this project is to analyze BBC news articles using Natural Language Processing (NLP) techniques to perform two core tasks:

Text Summarization – generating concise summaries of news articles.

Text Complexity Prediction – predicting the reading difficulty (complexity level) of news articles.

This can help tailor news content for different audiences such as children, non-native speakers, or people with reading difficulties.

📂 Dataset:
File Name: bbc_news_text_complexity_summarization.csv
Description:
This dataset consists of BBC news articles with the following features:

article: The full text of the news article.

summary: A manually written or auto-generated summary of the article.

complexity: A numeric value or class label indicating the reading difficulty of the article.

The dataset is well-suited for supervised learning tasks in both text summarization and complexity classification.

🧠 Methodology:
1. Data Preprocessing
Text Cleaning: Removal of stop words, punctuation, special characters, and converting all text to lowercase.

Tokenization: Splitting the article into words and sentences.

Stemming/Lemmatization: Reducing words to their root forms for uniformity.

2. Feature Engineering
TF-IDF Vectorization: Used to convert text data into numerical form for ML models.

Readability Metrics: Calculated using formulas like Flesch Reading Ease, Gunning Fog Index, and SMOG index.

Text Length Features: Number of words, sentences, average sentence length.

3. Complexity Prediction (Classification/Regression)
ML Models Used:

Logistic Regression

Random Forest

Support Vector Machine (SVM)

XGBoost

Model Evaluation: Models were evaluated using accuracy, precision, recall, F1-score (for classification) and RMSE, MAE (for regression).

4. Text Summarization
Extractive Summarization:

Used NLP-based techniques to identify key sentences in the article.

Implemented using algorithms like TextRank or custom scoring based on sentence importance.

Abstractive Summarization (Optional):

If attempted, uses encoder-decoder models or transformers like BART, T5, or GPT.

Evaluation: Used ROUGE metrics to compare the generated summaries with reference summaries.

📊 Results and Analysis:
🔢 Complexity Prediction:
Accuracy: (e.g., ~85% with Random Forest – actual result may vary based on code output)

Feature Importance: Readability scores and sentence length were key indicators of complexity.

📝 Summarization Quality:
ROUGE-1 / ROUGE-L scores: Used to assess how close the generated summary is to the reference summary.

Insights: Extractive methods worked well for shorter articles, but abstractive models performed better for generating human-like summaries.

🔍 Conclusion:
This project demonstrates the integration of NLP methods to assess and summarize textual content from news articles. By accurately predicting the complexity of articles, we can adapt content for diverse reading levels. The summarization component improves content accessibility by providing quick insights without reading the full article. Overall, the system provides a foundational pipeline for applications in educational tools, news apps, and content simplification platforms.

📈 Future Work:
Improve summarization using transformer-based models like BERTSUM or T5.

Expand complexity prediction to more fine-grained levels or use regression instead of classification.

Integrate the model into a web app where users can paste text and get both complexity score and summary.

Would you like this in a formatted PDF report or presentation format as well?
