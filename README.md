# Fake News Detection Model

This model can predict if a news article is real or fake.  
It uses Logistic Regression and TF‑IDF features.

## Accuracy
- Training: 98.6%
- Test: 97.9%

## Files in this repository
- `fake_news_model.pkl` – the trained model
- `tfidf_vectorizer.pkl` – text converter
- `Project1-FakeNewsPrediction.ipynb` – the complete notebook (includes training + prediction)

## Dataset
The model was trained on the [Scam Detection | Fake News Labelled Dataset from Kaggle](https://www.kaggle.com/datasets/noorsaeed/scam-detection-fake-news-labelled-dataset)

## How to use (step by step)

1. **Download everything from this repository**  
   - `fake_news_model.pkl`  
   - `tfidf_vectorizer.pkl`  
   - `Project1-FakeNewsPrediction.ipynb`

2. **Download the dataset** from the Kaggle link above  
   - You need to be logged into Kaggle.  
   - Download the file `train.csv`.

3. **Open Google Colab**  
   - Go to [colab.research.google.com](https://colab.research.google.com)  
   - Click **Upload** and select your notebook (`.ipynb` file)

4. **Upload the required files to Colab**  
   - In the left sidebar (folder icon), click **Upload**  
   - Upload: `fake_news_model.pkl`, `tfidf_vectorizer.pkl`, and `train.csv`

5. **Run all cells**  
   - Click **Runtime** → **Run all**  
   - The notebook will:
     - Load and preprocess the dataset
     - **Retrain the model** (to show accuracy scores)
     - **Then run the prediction cell** at the bottom

6. **Test your own news**  
   - The last cell will ask you to enter an **author** and a **title**  
   - Type any author and news title  
   - The model will print: `REAL NEWS` or `FAKE NEWS`

> **Note:** The notebook first retrains the model using the dataset. Then it loads your saved `.pkl` files to make the final prediction. This way you can verify the accuracy and also test custom inputs.
