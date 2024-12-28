# Finance News Aggregator

A Django-based web application that aggregates financial news from multiple sources including Reddit, Twitter, and Google News. Search once to get results from all platforms!

## Features

- Unified search across multiple platforms
- Reddit integration for community discussions
- Google News for latest articles
- Twitter integration for real-time updates
- Clean, modern UI with responsive design
- Error handling for failed API requests

## Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.8 or higher
- pip (Python package installer)

You'll also need these API credentials:
- Google Custom Search API key and Search Engine ID
- Twitter Bearer Token

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Mehtab-Cheema26/Finance-news-full-site.git
cd Finance-news-full-site
```

2. Create a virtual environment:
```bash
python -m venv venv
```

3. Activate the virtual environment:
- Windows:
```bash
venv\Scripts\activate
```
- Unix/MacOS:
```bash
source venv/bin/activate
```

4. Install required packages:
```bash
pip install django
pip install requests
pip install beautifulsoup4
pip install python-dotenv
pip install pandas
pip install httpx
pip install lxml
```

5. Create a .env file in the `buttonpython/buttonpython` directory with your API credentials:
```env
GOOGLE_API_KEY=your_google_api_key
GOOGLE_SEARCH_ENGINE_ID=your_search_engine_id
TWITTER_BEARER_TOKEN=your_twitter_bearer_token
```

## Running the Application

1. Navigate to the `buttonpython` directory:
```bash
cd buttonpython
```

2. Run the Django development server:
```bash
python manage.py runserver
```

3. Open your web browser and visit:
```
http://127.0.0.1:8000/
```

## Usage

1. On the homepage, you'll find a search bar.
2. Enter any finance-related topic (e.g., "AAPL", "Bitcoin", "Stock Market").
3. Click the search button.
4. View aggregated results from:
   - Reddit posts
   - Google News articles
   - Twitter posts

## Project Structure

```
buttonpython/
├── buttonpython/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── views.py
│   ├── google.py
│   ├── reddit_post.py
│   ├── twitter_post.py
│   └── wsgi.py
├── templates/
│   └── home.html
└── manage.py
```

## Troubleshooting

1. If you get API errors:
   - Verify your API credentials in the .env file.
   - Check if you've reached API rate limits.
   - Ensure your API keys have the correct permissions.

2. If the search returns no results:
   - Try different search terms.
   - Check your internet connection.
   - Verify the CSV files are being created properly.

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Reddit API
- Twitter API
- Google Custom Search API
- Django Framework
- Font Awesome for icons
- Google Fonts for typography
