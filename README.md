# 📊 Financial Sentiment Analysis using FinBERT

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.0+-red.svg)](https://streamlit.io/)

🚀 Analyze the sentiment of financial news headlines and articles using the state-of-the-art FinBERT model with an interactive Streamlit web application.

This project leverages FinBERT, a BERT-based model fine-tuned on financial text, to classify financial news into:

🟢 Positive  
🟡 Neutral  
🔴 Negative  

It provides real-time predictions along with probability scores via a clean and user-friendly web interface.

--------------------------------------------------

✨ FEATURES

🤖 Pre-trained FinBERT model for financial sentiment analysis  
⚡ Real-time sentiment predictions  
🌐 Interactive Streamlit web app  
📊 Probability scores for each sentiment class  
🚀 Fast and efficient inference on CPU/GPU  
📰 Web scraping and preprocessing of financial news data  

--------------------------------------------------

🛠 INSTALLATION

📌 Prerequisites
- Python 3.8 or higher
- pip package manager

⚙️ SETUP

1️⃣ Clone the repository

git clone https://github.com/022RaTiNdRa/Financial-Sentiment-Analysis-using-FinBERT.git
cd Financial-Sentiment-Analysis-using-FinBERT

2️⃣ Install dependencies

pip install -r requirements.txt

If requirements.txt is not present, install manually:

pip install torch transformers streamlit pandas numpy requests beautifulsoup4

--------------------------------------------------

▶️ USAGE

🌐 Web Application (Streamlit)

Run the Streamlit app:

streamlit run prediction.py

Open your browser and go to:

http://localhost:8501

You can:
✍️ Enter financial news headlines or articles  
📈 Get instant sentiment predictions  
📊 View probability scores for each sentiment class  

--------------------------------------------------

🧪 COMMAND LINE PREDICTION

from prediction import predict_sentiment

text = "Company X reports record profits this quarter."
sentiment, probabilities = predict_sentiment(text)

print(f"Sentiment: {sentiment}")
print(f"Probabilities: {probabilities}")

--------------------------------------------------

🗂 DATA PROCESSING

📰 Web Scraping

python web_scraping_and_preprocessing.py

🧠 Model Training (Optional)

python trained_model.py

--------------------------------------------------

📁 PROJECT STRUCTURE

Financial-Sentiment-Analysis-using-FinBERT/
|
|-- prediction.py
|-- trained_model.py
|-- web_scraping_and_preprocessing.py
|-- financial_news_combined.csv
|-- financial_news_preprocessed.csv
|-- scraped_business_insider_news.csv
|-- scraped_yahoo_data.csv
|-- .gitignore
|-- README.md

--------------------------------------------------

🤝 CONTRIBUTING

1. Fork the repository
2. Create your feature branch
   git checkout -b feature/AmazingFeature
3. Commit your changes
   git commit -m "Add AmazingFeature"
4. Push to the branch
   git push origin feature/AmazingFeature
5. Open a Pull Request

--------------------------------------------------

📜 LICENSE

This project is licensed under the MIT License.
See the LICENSE file for details.

--------------------------------------------------

🙏 ACKNOWLEDGMENTS

💡 ProsusAI for the FinBERT model  
🤗 Hugging Face for the Transformers library  
🎈 Streamlit for the web application framework  

--------------------------------------------------

📬 CONTACT

For questions or suggestions, please open an issue on GitHub.

⭐ If you find this project useful, consider starring the repository!
