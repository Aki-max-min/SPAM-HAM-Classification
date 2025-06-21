# SPAM-HAM-Classification
# Spam-Ham Email Classification

This project is a machine learning solution for classifying emails as **Spam** or **Ham** (not spam) using Python, scikit-learn, and natural language processing techniques.

## Features

- Data cleaning and preprocessing (removal of stopwords, lemmatization, etc.)
- Feature extraction using TF-IDF vectorization
- Multiple classification models (Random Forest, GaussianNB, MultinomialNB)
- Model evaluation and accuracy reporting
- Example code for predicting new emails

## How to Use

1. **Clone the repository:**
   ```
   git clone https://github.com/Aki-max-min/SPAM-HAM-Classification.git
   cd SPAM-HAM-Classification
   ```

2. **Install requirements:**
   ```
   pip install -r requirements.txt
   ```
   *(Create this file if needed, listing packages like `pandas`, `scikit-learn`, `nltk`, etc.)*

3. **Prepare your dataset:**
   - Place your dataset (e.g., `combined_data.csv`) in the project directory.
   - The dataset should have at least two columns: `label` and `text`.

4. **Run the notebook:**
   - Open `Code.ipynb` in Jupyter or VS Code.
   - Run all cells to train and evaluate the models.

5. **Predict new emails:**
   - Use the provided code to load the saved model and vectorizer, and classify new email samples.

## Notes

- The dataset file is **not included** in this repository. Please use your own data.
- The notebook demonstrates all steps from data loading to prediction.

## Example

```python
email = "Congratulations! You've won a free ticket. Click here to claim."
cleaned_email = clean_text(email)
X_input = tfidf.transform([cleaned_email]).toarray()
prediction = model.predict(X_input)
label = "Spam" if prediction[0] == 1 else "Ham"
print(f"Prediction: {label}")
```

## License

This project is for educational purposes.