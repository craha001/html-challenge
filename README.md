# html-challenge
## Module 11 Challenge Web Scraping

For this week's challenge, the goal was to use our understanding of html to scrape data from a specific website and perform an analysis on what was scraped. 

## Deliverable 1: Scrape titles and preview text from Mars news articles
When opening the MartianTemp folder there are two jupyter notebook files. Please open the file titled part_1_mars_news to obtain the code for this deliverable. 

### Step 1: Visiting the Website
Here is the url link for the website: https://static.bc-edx.com/data/web/mars_news/index.html. After opening up the website using our Jupyter Notebook, it is necessary to inspect the html code.

### Step 2: Scrape the Website
Using BeautifulSoup, we created an object that was then used to scrape all the text elements to get a better look at the classes for us to pull.

### Step 3: Store the Results
In this section, a function was created to pull the title of each article and their previews. This data was then stored in it's own dictionary which was then stored into a list. By doing so, we were able
to scrape the titles and their preview for the articles on the specified web page. 


## Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.
When opening the MartianTemp folder there are two jupyter notebook files. Please open the file titled part_2_mars_weather to obtain the code for this deliverable. In this section, we will be scraping a website for Mars weather data
and then converting it to a data frame using Pandas in order to create visualizations for analysis.

### 

