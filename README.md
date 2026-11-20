# 🎬 Movie Sentiment Analysis Dashboard

A Machine Learning-based web application that analyzes movie reviews and predicts whether the sentiment is **Positive or Negative** using Natural Language Processing (NLP) and Scikit-learn.

The application provides an interactive dashboard where users can enter movie titles and reviews, analyze sentiment, and view movie information.

## 🚀 Features

- **Sentiment Prediction:** Classifies movie reviews as Positive or Negative.
- **NLP Processing:** Uses text preprocessing and TF-IDF vectorization.
- **Machine Learning:** Uses Logistic Regression for sentiment classification.
- **Multiple Reviews:** Supports analyzing multiple reviews for a movie.
- **Confidence Score:** Displays prediction confidence and positive/negative probabilities.
- **Movie Information:** Fetches movie details using the OMDb API.
- **Interactive Dashboard:** Displays sentiment results, movie details, and review analysis.

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Backend | Flask, Flask-CORS |
| Machine Learning | Scikit-learn, Logistic Regression |
| NLP | TF-IDF, Text Preprocessing, NLTK |
| Data Processing | Pandas, NumPy |
| Frontend | HTML, CSS, JavaScript |
| External API | OMDb API |

## 🧠 How It Works

1. User enters a movie title and one or more reviews.
2. The application preprocesses the review text.
3. TF-IDF converts text into numerical features.
4. The trained Logistic Regression model predicts sentiment.
5. The dashboard displays Positive or Negative sentiment with confidence scores.
6. OMDb API provides additional movie information.

## 📂 Project Structure

```text
movie-sentiment-analysis/
│
├── app.py
├── train.py
├── index.html
├── movie.ipynb
├── sentiment_model.pkl
├── sentiment_pipeline.pkl
├── tfidf_vectorizer.pkl
├── requirements.txt
└── README.md
```

## ⚙️ Installation & Setup

**1. Clone the repository**

```bash
git clone https://github.com/abhayyysinghhh/movie-sentiment-analysis.git
```

**2. Navigate to the project directory**

```bash
cd movie-sentiment-analysis
```

**3. Create a virtual environment**

```bash
python -m venv venv
```

Activate it:

Windows:
```bash
venv\Scripts\activate
```

Mac/Linux:
```bash
source venv/bin/activate
```

**4. Install dependencies**

```bash
pip install -r requirements.txt
```

**5. Configure OMDb API**

Get an API key from [OMDb API](https://www.omdbapi.com/apikey.aspx).

Set the API key as an environment variable:

Windows PowerShell:
```powershell
$env:OMDB_API_KEY="your_api_key"
```

Mac/Linux:
```bash
export OMDB_API_KEY="your_api_key"
```

**6. Run the Flask application**

```bash
python app.py
```

Open `index.html` in your browser to access the dashboard.

## 🔗 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/health` | Checks backend and model status |
| POST | `/analyze` | Analyzes movie reviews and returns sentiment predictions |

## 🔮 Future Improvements

- Deploy the application to a cloud platform.
- Improve model accuracy through further evaluation.
- Explore advanced NLP and deep learning techniques.
- Add support for multiple languages.

## 👨‍💻 Technologies & Learning Outcomes

This project demonstrates practical implementation of Machine Learning, Natural Language Processing, Flask-based REST APIs, frontend integration, and external API connectivity.
