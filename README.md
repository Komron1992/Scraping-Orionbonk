Arvand Currency Fetcher
This Python script fetches up-to-date currency exchange rates from the arvand.tj public API.

📌 Features
Sends a GET request to https://arvand.tj/api/currencies/

Disables SSL certificate warnings for easier testing

Filters and returns only currencies with the type CASH_RATE

Outputs a dictionary with currency names and their buy/sell rates

🔧 Installation & Usage
Make sure you have Python 3.7 or higher installed

Install the required library:

pip install requests
Run the script:

python arvand.py
🧪 Example Output
{
    'USD': {'buy_rate': '10.80', 'sell_rate': '10.90'},
    'EUR': {'buy_rate': '11.70', 'sell_rate': '11.90'}
}
📁 Structure
fetch_currency_data_arvand() — main function to request and parse data from the API

Logs printed at each step: sending request, response status, filtering results

⚠️ Note
SSL verification is disabled (verify=False) — not recommended for production

If the API is unavailable or returns an error, the function returns None

📜 License
MIT — feel free to use and modify this script for your own projects.