# Sentiment Analysis of Google Reviews 🚀

## Project Overview
This project performs **Sentiment Analysis** on Google reviews using **Natural Language Processing (NLP)** techniques and the **Google Gemini Model** for advanced sentiment classification. The primary goal is to classify the sentiments of the reviews into three categories: **Positive**, **Neutral**, and **Negative**.

---

## Key Features
- **Sentiment Classification**: Automatically classifies reviews as Positive, Neutral, or Negative.
- **NLP Techniques**: Utilizes **Stemming**, **Lemmatization**, and **Text Preprocessing** for more accurate sentiment analysis.
- **Generative AI**: Integrated **Google Gemini Model** for enhanced sentiment prediction, improving accuracy through AI-driven insights.
- **Data Visualization**: Visualizes sentiment distribution to better understand the overall trend in user reviews.

---

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Project Structure](#project-structure)
4. [Model Explanation](#model-explanation)
5. [Technologies Used](#technologies-used)
7. [Contributing](#contributing)

---

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/sentiment-analysis-google-reviews.git
    cd sentiment-analysis-google-reviews
    ```

2. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Download the dataset (Google Reviews) using:
    ```python
    import gdown
    file_url = 'https://drive.google.com/uc?id=1FZXoO3-sfFBol2UbQWtvaXDmaQZ0ZgkD'
    gdown.download(file_url, 'reviews.csv', quiet=False)
    ```

---

## Usage

1. Preprocess the reviews by running:
    ```bash
    python preprocess_reviews.py
    ```

2. Train the sentiment analysis model:
    ```bash
    python train_model.py
    ```

3. Use the model to predict sentiment for new reviews:
    ```bash
    python predict_sentiment.py --review "I love this app!"
    ```

4. To run the project interactively:
    ```bash
    jupyter notebook
    ```

---

## Project Structure
```bash
├── data
│   └── reviews.csv             # Google reviews dataset
├── notebooks
│   └── sentiment_analysis_of_google_reviews.ipynb # Jupyter notebook for analysis
├── results
│   └── sentiment_distribution.png # Sentiment distribution visualization
└── README.md                   # Project readme
```
---

## Model Explanation

- Traditional ML Model: A Naive Bayes classifier is used to predict sentiments based on preprocessed review text.
- Generative AI Integration: The project also integrates Google Gemini Model, which adds a layer of advanced sentiment prediction based on AI-generated responses, making the model highly efficient and accurate.
- Text Preprocessing:
  - Stemming: Reduces words to their root forms.
  - Lemmatization: Further reduces words to their base or dictionary form.
---
 
## Technologies Used
- Python 🐍
- Natural Language Processing (NLP):
  - Stemming & Lemmatization
  - Tokenization & Stopword Removal
- Google Gemini API🤖
- Pandas, Matplotlib for data manipulation and visualization
- Scikit-learn for Machine Learning
---

## Contributing
Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add new feature`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

