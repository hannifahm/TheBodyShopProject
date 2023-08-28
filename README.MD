# The BodyShop Project

Data Scraping Project | **Nov 2022**

_This project consists of data scraping the skincare/beauty website, the BodyShop, with the goal of searching for sensitive-skin friendly products._

## Background Information

The main motivation for this project was personally driven. As someone with atopic dermatitis and an existing customer of the Bodyshop, the aim of this project was to find more products that were suitable for my skin.

First, to extract all relevant data on each skincare product, BeautifulSoup was utilised. Then, Selenium was used to perform **dynamic scraping** in order to list all the products available from each page on the website and thus, retrieve all information for each product. Data for each product was first saved in a dictionary then appended onto a list to finally create a DataFrame for further analysis. 

Analysis included searching for products that were sensitive-skin friendly and alcohol/fragrance-free and using an **ingredient-based recommendation system** to find recommendations similar to products that I own.


### Skills Used
* Data Scraping: dynamic scraping (BeautifulSoup, Selenium)
* Data Cleaning: Pandas (renaming columns, converting column dtypes, setting index, splitting rows etc.)
* Data Analysis: Matplotlib (word clouds), Scikit-learn (content-based recommendation system)

### Languages/Tools Used
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="70" height="70"/>
          

## Findings

Majority of the products aim to target sensitive skin as well as dry and dull skin. However, fragrance is one of the most common ingredients found in the products which can be problematic for individuals with extreme sensitive skin and skin conditions like eczema and dermatitis.

Out of 106 rows, a search for alcohol and fragrance-free products returns 12 rows; only 11% of the BodyShop's skincare products.
 
With the recommendation system, a product previously bought (_Aloe Calming Cream Cleanser_) was used as the input to find products in similarity. Due to the small sample size of products, recommended products were not as similar as expected. The recommended products fell under the Aloe branch, however, there was only one product of the same product type.

