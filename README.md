# ?? Financial Sentiment Analysis using FinBERT

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.0+-red.svg)](https://streamlit.io/)

> ?? **Analyze the sentiment of financial news headlines and articles using state-of-the-art FinBERT model and an interactive Streamlit web application.**

This project leverages the power of **FinBERT**, a pre-trained BERT model fine-tuned on financial texts, to classify financial news into three sentiment categories: **Positive** ??, **Neutral** ?, and **Negative** ??. Built with ease of use in mind, it provides real-time sentiment predictions with probability scores through a user-friendly web interface.

## ? Features

- ?? **Pre-trained FinBERT Model**: Utilizes ProsusAI'"'"'s FinBERT for accurate financial sentiment analysis
- ? **Real-time Predictions**: Get instant sentiment analysis with confidence scores
- ?? **Interactive Web App**: Built with Streamlit for seamless user interaction
- ?? **Probability Scores**: View detailed probability distributions for each sentiment class
- ?? **Fast & Efficient**: Optimized for quick inference on CPU/GPU
- ?? **Data Processing**: Includes web scraping and preprocessing scripts for financial news data

## ??? Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup
1. **Clone the repository**:
   ```bash
   git clone https://github.com/022RaTiNdRa/Financial-Sentiment-Analysis-using-FinBERT.git
   cd Financial-Sentiment-Analysis-using-FinBERT
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

   > ?? **Note**: If `requirements.txt` is not present, install the following core packages:
   - `torch`
   - `transformers`
   - `streamlit`
   - `pandas`
   - `numpy`
   - `requests`
   - `beautifulsoup4`

## ?? Usage

### Web Application
Run the Streamlit web app for interactive sentiment analysis:

```bash
streamlit run prediction.py
```

Navigate to `http://localhost:8501` in your browser to:
- ?? Enter financial news headlines or articles
- ?? Get instant sentiment predictions
- ?? View probability scores for each sentiment class

### Command Line Prediction
Use the prediction script directly:

```python
from prediction import predict_sentiment

text = "Company X reports record profits this quarter."
sentiment, probabilities = predict_sentiment(text)
print(f"Sentiment: {sentiment}")
print(f"Probabilities: {probabilities}")
```

### Data Processing
Process and analyze financial news data:

1. **Web Scraping**:
   ```bash
   python web_scraping_and_preprocessing.py
   ```

2. **Model Training** (if needed):
   ```bash
   python trained_model.py
   ```

## ?? Project Structure

```
Financial-Sentiment-Analysis-using-FinBERT/
¦
+-- prediction.py                 # Main prediction script and Streamlit app
+-- trained_model.py              # Model training utilities
+-- web_scraping_and_preprocessing.py  # Data scraping and preprocessing
+-- financial_news_combined.csv   # Combined financial news dataset
+-- financial_news_preprocessed.csv  # Preprocessed news data
+-- scraped_business_insider_news.csv  # Business Insider scraped data
+-- scraped_yahoo_data.csv        # Yahoo Finance scraped data
+-- .gitignore                    # Git ignore file
+-- README.md                     # Project documentation
```

## ?? Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m '"'"'Add some AmazingFeature'"'"'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## ?? License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ?? Acknowledgments

- **ProsusAI** for the FinBERT model
- **Hugging Face** for the Transformers library
- **Streamlit** for the amazing web app framework

## ?? Contact

For questions or suggestions, please open an issue on GitHub.

---

? **Star this repo if you find it useful!**
