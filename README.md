# Al-Jazzera-News-Scraper AND Emailer
A simple automation script that scrapes the top news stories from Al Jazeera English and emails them to you daily. It fetches each headline and URL, then sends them using Gmail SMTP to your chosen email address.

This was originally built to automate my own morning news routine instead of visiting the site manually, the script sends me the day’s top headlines so I can quickly scan and open only the ones that interest me.

# Features
1. Scrapes top news from Al Jazeera English.
2. Sends results via email automatically.
3. Configurable time for daily updates.
4. Runs headless using Selenium for full automation.
5. Stores settings locally for reusability.

# Setup Instructions
Clone or download this repository.

Install dependencies:
pip install -r requirements.txt

Run the script:
python3 news.py

Note: This script works best when deployed on a cloud or always-on device (e.g. Raspberry Pi)

# Getting Email Ready
Using Gmail, you’ll need to set up App Passwords (not your regular password).
https://support.google.com/accounts/answer/185833?sjid=4834380145672657079-NC
Once generated, use the 16-character password when the script prompts for your credentials.

# How It Works
Reads or creates a settings file at lib/settings.json.
Schedules a scraping task based on your preferred time.
Uses Selenium to fetch the latest headlines.
Sends the results via Gmail SMTP.

# Support
If you find this useful, consider giving the project a Star on GitHub it really helps!


