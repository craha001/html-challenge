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

### Step 1: Visiting the Website
Here is the url link for the website: https://static.bc-edx.com/data/web/mars_facts/temperature.html. Again, using html in our jupyter notebook to open the site in order to identify which elements we would like to scrape.

### Step 2: Scrape the Table
Once the site has been visited one can notice a table with our necessary data which will need to be scraped into our notebook in order for us to make our data frame. Again, create a BeautifulSoup object in order to find the ID and class to be stored
into a variable for our analysis later.

### Step 3: Store the Data
Here an empty list is created to store the data from the columns. Once the list is created, it can be converted into a datafram using pandas which will then be used to perform our analysis.
Below is a list of the columns and their descriptions:

id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location

### Step 4: Prepare Data for Analysis
In this step, our data in the dataframe are all currently objects. In order to perform our analysis using datetime and astypes our data frame is converted to the following:

id: object
terrestrial_date: datetime
sol: int32
ls: int32
month: int32
min_temp: float64
pressure: float64

### Step 5: Analyze the Data
Analyze the dataset by using Pandas functions to answer the following questions:

1. How many months exist on Mars?  
   12 months
2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?  
   1867 days
3. What are the coldest and the warmest months on Mars (at the location of Curiosity)?   
   Using a bar chart found in the code, the average coldest month on Mars was month 3 and the average warmest
   month on Mars was month 8.
4. Which months have the lowest and the highest atmospheric pressure on Mars?   
   Again using a bar chart found in the code, the average highest atmospheric pressure month on Mars was
   month 9 while the lowest pressure month on Mars was month 6.
5. About how many terrestrial (Earth) days exist in a Martian year?   
   By creating a plot where we plotted martian days versus minimum temperature on Mars, the graph creates
   a sinuisoidal shape. With this plot, by following the cycle and change in temperature over time the
   visualization showed that a Martian year is 600-700 days long. 


## Contributions
I collaborated on this assignment with Nicolas Ortega and Brendan Golden.
