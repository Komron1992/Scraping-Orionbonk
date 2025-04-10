🏦 Amonatbonk Currency Fetcher
This Python script fetches current exchange rates from the official Amonatbonk API, specifically targeting individual customer rates.

📌 Features
Sends a GET request to the Amonatbonk backend API

Parses and returns exchange rates for individuals

Simple and lightweight — no external dependencies other than requests

🔧 Installation
Make sure Python 3.6+ is installed

Install the required package:


pip install requests

🚀 Usage

python amonatbonk.py

✅ Example Output

{
  "USD": {"buy": "10.80", "sell": "10.90"},
  "EUR": {"buy": "11.70", "sell": "11.95"},
  "RUB": {"buy": "0.120", "sell": "0.126"}
}

🧠 How It Works

The script sends a GET request to:


https://amonatbonk.tj/bitrix/templates/amonatbonk/ajax/ambApi.php

It extracts the individuals section from the JSON response

Returns a dictionary of exchange rates

⚠️ Notes
If the API is unavailable or returns an error, the script prints an error message and returns an empty dictionary

The URL contains a query parameter (timestamp-like) which can be static or dynamic — in most cases it's ignored by the server

📜 License
MIT — use freely in your own projects.