# Arabic-Hate-Speech-Detection
This study Works on Arabic hate speech detection using BERT-based Transformers, including MARBERT, BERT-multilingual, AraBERTv0.2-Twitter, CAMeLBERT, QARiB, and SaudiBERT, evaluated on OSACT, LAHS, and arHate datasets. 

## 📚 Datasets

This project uses the following publicly available datasets for Arabic hate speech detection:

1. **[arHate Dataset](https://github.com/ramzi-kh/arHateDetector/tree/main/Datasets)**  
   A dataset for Arabic hate speech detection, sourced from tweets and annotated for hate speech and offensive language.

2. **[OSACT5 Dataset](https://osact5-lrec.github.io/)**  
   A dataset provided by the OSACT-5 shared task, focusing on hate speech and offensive language detection in Arabic.

3. **[LAHS Dataset](https://www.kaggle.com/datasets/ziedzen/levantine-arabic-hate-speech-detection-corpus?select=Arabic_Tweets_dataset.csv)**  
   The Levantine Arabic Hate Speech (LAHS) detection corpus, consisting of annotated tweets written in Levantine Arabic.

## **Pipeline**

1. **Dataset Collection**  
   The datasets are downloaded and stored locally in a directory named `datasets`.

2. **Text Pre-processing**  
   - Clean Arabic text by removing URLs, emojis, and special symbols.
   - Normalize the text to handle variations in spelling and diacritics.
   
3. **Data Partitioning**  
   - Split the data into **80% for training** and **20% for testing**.

4. **Hyperparameter Tuning**  
   - Fine-tune key hyperparameters such as batch size, learning rate, and weight decay.

5. **Model Training**  
   - Train various Arabic BERT-based models, including MARBERT, BERT-multilingual, AraBERTv0.2-Twitter, CAMeLBERT, QARiB, and SaudiBERT, using the training set.

6. **Evaluation**  
   - Evaluate model performance on the test set using metrics like accuracy, precision, recall, and F1-score.

7. **Output Classification**  
   - The models classify input text as either **Hate Speech** or **Non-Hate Speech**.

8. **Hyperparameter optimization**  
   - The models apply Grid search and Bayesian optimization.
    


<p align="center">
  <img src="Implementation steps.png" alt="Model Architecture" width="600">
</p>
