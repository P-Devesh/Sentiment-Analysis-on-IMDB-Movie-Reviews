# Sentiment-Analysis-on-IMDB-Movie-Reviews

# Sentiment Analysis on IMDB Movie Reviews

## Project Overview
This project builds a deep learning model using LSTM (Long Short-Term Memory) networks to classify IMDB movie reviews as positive or negative. It uses text preprocessing, tokenization, and embedding layers to transform raw text into meaningful numeric data for training.

## Dataset
- IMDB movie reviews dataset with labeled positive and negative sentiments.
- The reviews are tokenized and padded to a fixed length of 200 words.
- Top 5000 most frequent words are used for building the vocabulary.

## Model Architecture
- **Embedding Layer:** Converts each word into a 128-dimensional vector.
- **LSTM Layer:** Processes sequences of word vectors to capture temporal dependencies with 128 units.
- **Dense Layer:** Outputs a single value between 0 and 1 using sigmoid activation indicating sentiment polarity.

## Training
- Optimizer: Adam  
- Loss Function: Binary Crossentropy  
- Metrics: Accuracy  
- Epochs: 5 (can be adjusted)

## How to Run
1. Install dependencies:
pip install -r requirements.txt

markdown
Copy
Edit
2. Run the training script:
python train.py

yaml
Copy
Edit

## Key Learnings
- Text preprocessing: Tokenization and padding for uniform input size.
- Word embedding: Representing words in a continuous vector space.
- Sequential modeling with LSTM to capture context in text.
- Model evaluation using accuracy metric.

## Validation vs Testing
- Validation set helps tune the model during training to avoid overfitting.
- Test set is used for final unbiased evaluation after training.

## Future Improvements
- Incorporate text cleaning (lemmatization, removing stopwords).
- Use pretrained embeddings like GloVe or Word2Vec.
- Hyperparameter tuning for improved accuracy.
- Deploy the model as a web app using frameworks like Streamlit or Flask.

---

## License
This project is licensed under the MIT License.

---

Feel free to customize this README further with screenshots, examples, or additional instructions.

If you want, I can also help generate a `requirements.txt` for you!
