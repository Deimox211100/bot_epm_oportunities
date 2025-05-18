# EPM Opportunities Scraper

This project is a bot that scrapes open procurement opportunities from the [EPM](https://portalesepm.epm.com.co/TeCuento/ProcesosComprasMenoresVigentes/ConsultarProcesosCompras.aspx) website. It uses Selenium to automate browser actions, extract relevant process data, filter by keywords, and export the results to a CSV file.

## Features

- Automates Chrome browser to navigate and interact with the EPM procurement portal.
- Extracts all open process data from the site.
- Filters opportunities by configurable keywords.
- Exports filtered results to a CSV file in the `data/` directory.

## Requirements

- Python 3.7+
- Google Chrome browser
- ChromeDriver (compatible with your Chrome version)
- The following Python packages:
  - `selenium`
  - `pandas`

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/bot_epm_oportunities.git
   cd bot_epm_oportunities
   ```

2. **Install dependencies:**
   ```sh
   pip install pandas selenium
   ```

3. **Download [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/downloads)** and ensure it is in your PATH.

## Usage

1. Open and run the Jupyter notebook [`epm_scrapper.ipynb`](epm_scrapper.ipynb).
2. The bot will:
   - Open Chrome and navigate to the EPM procurement page.
   - Accept the terms and load the list of open processes.
   - Extract and filter the data by keywords (edit the `key_words` list in the notebook to customize).
   - Save the filtered results as a CSV file in the `data/` directory, named with the current date.

## Customization

- **Keywords:**  
  Edit the `key_words` list in the notebook to filter for different opportunities.

## Output

- Filtered opportunities are saved as CSV files in the `data/` folder, e.g., `PROCESOS_EPM_YYYY-MM-DD.csv`.

## License

This project is for educational and personal use.

## Maintainers

See [CODEOWNERS](.github/CODEOWNERS).
