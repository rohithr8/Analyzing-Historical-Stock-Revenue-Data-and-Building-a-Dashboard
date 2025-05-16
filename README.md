# Analyzing-Historical-Stock-Revenue-Data-and-Building-a-Dashboard
📈 Final Assignment – Stock and Revenue Data Analysis
Overview
This project analyzes historical stock price data and quarterly revenue for Tesla (TSLA) and GameStop (GME) using Python. It demonstrates how to fetch financial data, clean and process it, and visualize trends using custom graphing functions.

The project uses data from:

Yahoo Finance API via the yfinance package

HTML financial tables hosted by IBM via requests, BeautifulSoup, and pandas.read_html()

📂 Project Structure
File / Folder	Description
Final Assignment.ipynb	Main notebook containing all analysis, code, and visualizations
README.md	Project description and usage
make_graph()	Custom function to display dual-axis plots of stock price and revenue

🔧 Tools & Libraries Used
pandas

yfinance

requests

BeautifulSoup4

plotly.graph_objects (for interactive plotting)

🔍 What It Does
Retrieves historical stock data for Tesla and GameStop using yfinance

Scrapes quarterly revenue tables from HTML pages

Cleans and processes revenue data (removing $, ,, and nulls)

Visualizes:

Stock Closing Prices over time

Quarterly Revenue over time

Interactive dual-plot graphs for both Tesla and GameStop

🧪 How to Run
Install dependencies:

bash
Copy
Edit
pip install yfinance pandas beautifulsoup4 plotly lxml
Run the Jupyter Notebook:

bash
Copy
Edit
jupyter notebook Final\ Assignment.ipynb
Ensure internet access is available (to fetch live stock data and HTML content).

📊 Graphs Generated
make_graph(tesla_data, tesla_revenue, "Tesla")

make_graph(gme_data, gme_revenue, "GameStop")

Each graph:

Shows stock prices up to June 2021

Plots revenue and closing price on a shared time axis

✅ Data Sources
Tesla Stock & Revenue: Yahoo Finance, IBM Course-hosted HTML

GameStop Stock & Revenue: Yahoo Finance, IBM Course-hosted HTML

📌 Notes
The code handles deprecated warnings (e.g., infer_datetime_format) gracefully.

Revenue is converted to float after stripping currency symbols.

Plots are interactive via Plotly.

