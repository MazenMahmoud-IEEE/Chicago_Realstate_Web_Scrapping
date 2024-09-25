# Chicago Real Estate Web Scraping Project

## Overview

This project scrapes real estate data from Century21's Chicago listings using Python. It collects information on property prices, number of bedrooms and bathrooms, square footage, and addresses. The scraped data is then compiled into a pandas DataFrame and exported as a CSV file.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Output](#output)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

- Python 3.x
- Jupyter Notebook (optional, but recommended)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/chicago-real-estate-scraper.git
   cd chicago-real-estate-scraper
   ```

2. Install the required packages:
   ```
   pip install requests beautifulsoup4 pandas ipython
   ```

## Usage

1. Open the Jupyter Notebook `Chicago_Real_Estate_Web_scrapping.ipynb`.
2. Run all cells in the notebook sequentially.
3. The scraped data will be saved as `output.csv` in the project directory.

## Project Structure

- `Chicago_Real_Estate_Web_scrapping.ipynb`: Main Jupyter Notebook containing the scraping code.
- `output.csv`: CSV file containing the scraped real estate data.
- `README.md`: This file, containing project documentation.

## How It Works

1. **Importing Libraries**: The script uses `requests` for making HTTP requests, `BeautifulSoup` for parsing HTML, and `pandas` for data manipulation.

2. **Fetching First Page**: The script starts by scraping the first page of listings to set up the data structure.

3. **Fetching Remaining Pages**: It then loops through the remaining pages (up to 134) to collect data from all listings.

4. **Data Extraction**: For each property listing, the script extracts:
   - Number of bedrooms
   - Number of bathrooms
   - Square footage
   - Address
   - Price

5. **Data Processing**: The extracted data is cleaned and converted to appropriate data types.

6. **Creating DataFrame**: All collected data is compiled into a pandas DataFrame.

7. **Exporting to CSV**: The DataFrame is exported to a CSV file named `output.csv`.

## Output

The script generates a CSV file with the following columns:

- `bed rooms`: Number of bedrooms
- `baths`: Number of bathrooms
- `square feet`: Property size in square feet
- `address`: Full address of the property
- `price`: Listing price of the property

## Contributing

Contributions to improve the script or extend its functionality are welcome. Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
