# Image Scraper

This Python script allows you to scrape images from Google Images based on a search term using Selenium and Chrome WebDriver.

## Setup

1. Install the required dependencies by running `pip install selenium pillow requests`.
2. Ensure that you have Google Chrome installed on your machine.
3. Check your Google Chrome version by going to the three dots menu -> Help -> About Google Chrome.
4. Download the corresponding Chrome WebDriver from [here](https://chromedriver.chromium.org/downloads). Make sure to download the version that matches your Chrome version.
5. Place the downloaded Chrome WebDriver executable in the same folder as this script.

## Usage

1. Run the script using `python image_scraper.py`.
2. Enter the name of the item you want to search for when prompted.
3. Enter the number of images you want to scrape when prompted.
4. The script will create a folder with the search term as the name (all lowercase with spaces replaced by underscores) in the current directory.
5. The images will be downloaded and saved in the created folder.

Note: The script uses Chrome WebDriver to automate the Google Images search and retrieve the image URLs. It then uses the `requests` library to download and save the images locally.

## Limitations and Improvements

- The script relies on the structure and CSS selectors of the Google Images page, which may change over time. If the script stops working, check if the structure of the Google Images page has been modified and update the CSS selectors accordingly.
- The script currently downloads the images sequentially. It can be optimized to download images in parallel using multiple threads or asynchronous requests for faster scraping.
- Error handling can be improved to handle exceptions during the scraping process and provide more informative error messages.
- The script could be extended to support other search engines or image sources by modifying the code to scrape from different websites.

## License

This project is licensed under the [MIT License](LICENSE).

---
