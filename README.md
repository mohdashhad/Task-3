# Task-3
This project scrapes travel-related websites about the Maldives, extracts high-quality keywords using Natural Language Processing (NLP) techniques, classifies them by tail type, and saves the results to an Excel file or Google Sheets. It supports automated scheduling to run daily.

📌 Objectives
Extract relevant travel keywords like:

Places to visit in Maldives for couples

Maldives travel guide, etc.

Categorize keywords into:

Short-tail (2 words)

Mid-tail (3 words)

Long-tail (4+ words)

Schedule automatic keyword scraping and export results

📁 Project Structure
bash
Copy
Edit
maldives-keyword-scraper/
│
├── maldives_200_keywords.xlsx       # Final output with 200 sample keywords
├── maldives_keywords_scraper.py     # Main scraping + NLP + automation script
├── requirements.txt                 # Required Python packages
└── README.md                        # Project documentation
🛠️ Features
✅ Web scraping using requests and BeautifulSoup

✅ NLP keyword extraction using RAKE

✅ Categorization by tail type

✅ Output to Excel (.xlsx)

✅ Optional Google Sheets integration

✅ Automation using schedule library (daily or custom time)

🌐 Target URLs
Example sources scraped:

tripadvisor.in

holidify.com

makemytrip.com

thrillophilia.com

traveltriangle.com

thomascook.in

yatra.com, etc.

🔧 Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/maldives-keyword-scraper.git
cd maldives-keyword-scraper
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
requirements.txt
text
Copy
Edit
requests
beautifulsoup4
rake-nltk
pandas
openpyxl
schedule
Optional for Google Sheets:

text
Copy
Edit
gspread
oauth2client
▶️ How to Run the Script
One-time run
bash
Copy
Edit
python maldives_keywords_scraper.py
Scheduled Daily Automation
The script is pre-configured to run daily at 9:00 AM:

python
Copy
Edit
schedule.every().day.at("09:00").do(scrape_and_analyze)
You can change it to hourly/weekly as needed.
