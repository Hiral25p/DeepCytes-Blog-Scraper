
# DeepCytes Blog Scraper

The DeepCytes Blog Scraper is a Jupyter Notebook tool for scraping and analyzing blog articles from various sources. Follow the steps below to set up and use the scraper.

# Generated Sheet
(https://docs.google.com/spreadsheets/d/1Gly5V-lVWRGMaaHaF0RW2Skub8DZEwajOUmb_wjyg08/edit?usp=sharing)

## Clone the Repository
To get started, clone the repository to your local machine:
```
git clone https://github.com/yourusername/DeepCytes-Blog-Scraper.git
```

## Navigate to the Project Folder
```
cd DeepCytes-Blog-Scraper
```

## Project Structure
```
DeepCytes-Blog-Scraper/
├─ DeepCytes_Blog_Scraper (1).ipynb
├─ credentials (1).py
└─ readme.md
```

## Setup

### Install Dependencies
Ensure you have the following libraries installed:

- requests
- pandas
- datetime
- gspread
- google-auth
- beautifulsoup4

You can install them using:
```
pip install requests pandas gspread google-auth beautifulsoup4
```
Use your own enviornment variables as per ```.env.example```
### API Configuration (for Google Sheets Integration)
If the notebook interacts with Google Sheets, set up Google Sheets API credentials by following these steps:

- Create a Google Cloud project and enable the Google Sheets API.
- Download the service account credentials JSON file and save it to your project directory.
- Rename the JSON file as `credentials.py` (or adjust the notebook to match your file’s name).
- Ensure the Google Sheets document is shared with the email in your service account.

### NewsAPI Key (for News Articles)
Go to [NewsAPI](https://newsapi.org/) and sign up for a free account.
Once registered, go to the API Key section in your dashboard.
Copy the API key provided.
In the Jupyter Notebook, store this key as a variable, or add it to an `.env` file if you prefer, to keep it secure:
```python
NEWSAPI_KEY = "your_newsapi_key_here"
```

## Running the Scraper
Open the notebook:
```
jupyter notebook DeepCytes_Blog_Scraper.ipynb
```

Execute the cells in sequence to start the scraping and analysis process.
