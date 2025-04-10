# 🏦 Scraping Orionbonk Currency Rates

This Python script scrapes real-time currency exchange rates from the official website of [Orionbonk](https://oriyonbonk.tj/ru).

## 📌 Features

- Fetches the latest exchange rates (buy/sell) directly from Oriyonbonk’s homepage
- Parses HTML using `BeautifulSoup` and `lxml`
- Returns results as a clean Python dictionary

## 🛠️ Built With

- Python 3.x
- [requests](https://pypi.org/project/requests/)
- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
- [lxml](https://pypi.org/project/lxml/)

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/Komron1992/Scraping-Orionbonk.git
cd Scraping-Orionbonk

2. Install dependencies:

pip install -r requirements.txt

🚀 Usage

Simply run the script:

python orionbonk.py

💡 Example Output:

{
    'USD': {'buy_price': '10.80', 'sell_price': '10.90'},
    'EUR': {'buy_price': '11.50', 'sell_price': '11.70'},
    ...
}

📄 License
This project is intended for educational and informational purposes only.