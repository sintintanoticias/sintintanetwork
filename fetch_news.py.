import requests
import json

API_KEY = '7005a6609b9a4b0a8c3a0e35124817d4'
URL = 'https://newsapi.org/v2/top-headlines'

def fetch_news():
    params = {
        'apiKey': API_KEY,
        'language': 'es',
        'country': 'es'
    }
    response = requests.get(URL, params=params)
    news_data = response.json()

    with open('news.json', 'w', encoding='utf-8') as f:
        json.dump(news_data, f, ensure_ascii=False, indent=4)

if __name__ == "__main__":
    fetch_news()
