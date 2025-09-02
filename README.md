# Emotion-analysis-with-AI
Today, I want to share with you a small but exciting project I've been working on. I wanted to develop an AI model that can automatically analyze the sentiment (Negative, Neutral, Positive) of sentences/comments written in Turkish.

To run the code in the gitignore file, 
    1-first you should install the pandas, numpy, datasets, transformers, evaluate, torch, scikit-learn, matplotlib, and seaborn libraries.
    2-You should download the CSV file required for model training from the address below and rename the file to “data.csv”.
 https://www.kaggle.com/datasets/burhanbilenn/duygu-analizi-icin-urun-yorumlari?resource=download
    3-After the code finishes running, open a new py file and write the following code:  from transformers import pipeline

sentiment_pipe = pipeline(
    “text-classification”,
    model="./sentiment-tr",
    tokenizer="./sentiment-tr")


print(sentiment_pipe(“Test Sentence”))
