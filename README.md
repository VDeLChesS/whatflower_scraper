# Flower Species Scraper

This Python script scrapes all the flower species and their images from the website [https://whatflower.net/](https://whatflower.net/). The images are downloaded and then saved locally in an ``` images ```directory.

## About the Target Website

[https://whatflower.net](https://whatflower.net/) is a platform that showcases various flower species with descriptions and images. It provides a visual guide to flower identification and serves as a useful resource for botanists, gardeners, and flower enthusiasts.

## What the Script Does

1. **Web Scraping**:
   - The script retrieves the main page of the website and parses its HTML content.
   - It identifies flower species and their associated images by targeting specific HTML elements.

2. **Image Downloading**:
	- For each flower species found, the script downloads its image.
 	- Images are saved in a folder named ``` images ``` with filenames corresponding to the species names.

3. **Error Handling**:

	- Ensures that the ``` images ```  directory exists.
	- Handles potential errors during image downloading and file saving.

## How the Script Works
- Requests: Fetches the HTML content of the target webpage.
- BeautifulSoup: Parses the HTML to extract the required information, such as species names and image URLs.
- File I/O: Saves the downloaded images to the local filesystem.
 
## Key Functions:

1. ```save_image(species_name, img_url)```:
   - Downloads an image from the given URL and saves it as a ``` .png ``` file in the ``` images ``` directory.
2. ```scrape_species()```:
   - Scrapes the main page of https://WhatFlower.net to extract flower species names and image URLs.
3. ```main()```:
   - The entry point for the script. Calls ``` scrape_species() ``` to start the scraping process.

## Dependencies

1. This script requires the following external Python libraries:
   *```requests```: For making HTTP requests to the website
  
			pip install requests

	*```beautifulsoup4 ```: For parsing HTML content

			pip install beautifulsoup4
	  
## Usage

1. **Install Dependencies:**
	* Make sure you have Python installed.
	+ Install the required libraries using the commands listed in the Dependencies section.

2. **Run the Script:**
 	* Save the script to a .py file (e.g., flower_scraper.py).
	* Run the script in your terminal:
		``` bash Copy code
		python flower_scraper.py
3. **Check the Images:**
	* After running the script, check the ``` images ``` directory in the same folder as the script. All the flower images will be saved there.

## Notes
- Ensure you have a stable internet connection to access the target website and download images.
- The website's structure might change, so the script may need updates to handle future changes in the HTML layout.
 
## License
This script is provided "as-is" for educational and personal use. Please ensure compliance with WhatFlower.net's terms of use when running this script.
