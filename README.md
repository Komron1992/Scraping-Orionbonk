🕸️ Imon Currency Scraper (Selenium)
This Python script uses Selenium to scrape real-time currency exchange rates (Dollar, Euro, Ruble) from the official Imon.tj website.

📌 Features
Automates Chrome browser using Selenium

Runs in headless mode (no GUI)

Extracts currency buy/sell rates for:

💵 Dollar

💶 Euro

🇷🇺 Russian Ruble

Optimized for performance (images disabled, long timeouts)

Uses webdriver-manager to auto-install ChromeDriver

🔧 Installation
Install required packages:

pip install selenium webdriver-manager
Optional: If you don’t have Google Chrome installed, download and install it first.

🚀 Usage
python imon_scraper.py
Example output:
{
  'Dollar': {'buy': '10.80', 'sell': '10.90'},
  'EURO': {'buy': '11.70', 'sell': '11.90'},
  'Ruble': {'buy': '0.120', 'sell': '0.125'}
}
🧠 How It Works
Opens https://www.imon.tj/ in a headless Chrome browser

Waits up to 120 seconds for currency elements to load

Parses currency blocks using class names, inner HTML, and XPath

Returns a dictionary of currency data (or an empty one on error)

⚠️ Notes
The script is designed to be resilient but may break if Imon.tj changes their HTML structure.

Headless scraping is resource-light but slower than direct API access.

The website uses SVG icons to identify currencies (dollar.svg, euro.svg, rub.svg)

✅ Best Practices
Always wrap scraping in try-except blocks (already done here)

Respect websites' robots.txt and scraping policies

Avoid sending frequent requests — cache results if possible

📜 License
MIT — free to use, share, and modify.

