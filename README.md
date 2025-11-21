# Pakistani E-commerce Marketplace Analyzer

This project is a price comparison and intelligence tool for Pakistani e-commerce platforms. It scrapes product data from Daraz.pk and searches other local marketplaces (PriceOye, OLX, Telemart, Shophive, etc.) using Serper.dev. The system analyzes prices, generates comparison reports, and provides market insights using Groq LLM.

## How It Works
- Scrapes product details from Daraz.pk using Playwright
- Searches other platforms via Serper.dev API
- Analyzes and compares prices using Groq LLM
- Generates markdown reports and saves results to a local SQLite database
- Offers both a CLI and a Streamlit web interface for interactive use

## APIs Used
- Serper.dev: For searching Pakistani e-commerce sites
- Groq: For AI-powered analysis and report generation

## Setup & Usage
1. Clone the repo and create a Python virtual environment
2. Install dependencies: `pip install -r requirements.txt`
3. Install Playwright browsers: `playwright install chromium`
4. Add your API keys to a `.env` file:
	- GROQ_API_KEY=...
	- SERPER_API_KEY=...
5. Run the Streamlit app: `streamlit run streamlit_app.py`
	- Or use the CLI: `python main.py "product name"`

## License
MIT LicenseS