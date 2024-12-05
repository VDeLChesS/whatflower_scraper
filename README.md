# 🌸 Flower Species Scraper

--- 

This Python script scrapes all the flower species and their images from the website [https://whatflower.net/](https://whatflower.net/). The images are downloaded and then saved locally in an ``` images ```directory.

## 🖼️ About the Target Website

[**WhatFlower.net**](https://whatflower.net) is a platform dedicated to showcasing various flower species, complete with descriptions and images. It serves as an invaluable resource for:
- Botanists
- Gardeners
- Flower enthusiasts  
 
The website is both a visual guide and a tool for flower identification.

---

## 🛠️ Features of the Script

### 🌐 **Web Scraping**
- Retrieves the main page of the website and parses its HTML content.
- Extracts flower species names and their associated images by targeting specific HTML elements.

### 📥 **Image Downloading**
- Downloads an image for each flower species found on the site.
- Saves images in an `images` directory with filenames corresponding to the species names.

### ⚙️ **Error Handling**
- Ensures that the `images` directory exists before downloading.
- Manages potential issues during image downloading and file saving.

---

## 🔍 How the Script Works
- Requests: Fetches the HTML content of the target webpage.
- BeautifulSoup: Parses the HTML to extract the required information, such as species names and image URLs.
- File I/O: Saves the downloaded images to the local filesystem.
 
### Key Functions:

- **`save_image(species_name, img_url)`**
  - Downloads an image from the provided URL and saves it as a `.png` file in the `images` directory.
- **`scrape_species()`**
  - Scrapes the main page of [WhatFlower.net](https://whatflower.net) to extract flower species names and image URLs.
- **`main()`**
  - Entry point of the script. Executes `scrape_species()` to initiate the scraping process.

---


## 📦 Dependencies

This script requires the following external Python libraries:

1. **`requests`**: For making HTTP requests to the website  
   ```bash
   pip install requests

2. **`beautifulsoup4`**: For parsing HTML content
   ```bash
   pip install beautifulsoup4
	  
## ▶️ Usage

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

## 📝 Notes
- Ensure you have a stable internet connection to access the target website and download images.
- The website's structure might change, so the script may need updates to handle future changes in the HTML layout.
 
## 📖 License
This script is provided "as-is" for educational and personal use. Please ensure compliance with WhatFlower.net's terms of use when running this script.
