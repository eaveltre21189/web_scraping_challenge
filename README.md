# web_scraping_challenge

## Deliverable 1: Scrape Titles and Preview Text from Mars News
<br>

### Step 1: Visit the Website
<br>

* Use automated browsing to visit the [Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html). Inspect the page to identify which elements to scrape.
<br><br>

### Step 2: Scrape the Website
<br>

* Create a Beautiful Soup object and use it to extract text elements from the website.
<br><br>

### Step 3: Store the Results
<br>

* Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
* Store each title-and-preview pair in a Python dictionary, and give each dictionary two keys: `title` and `preview`.
* Store all the dictionaries in a Python list.
* Print the list in your notebook.
<br><br>

### Step 4:  Store the Results in a File
<br>

* Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)
<br><br>
    
    **Note:**  To write the results to a JSON file, I followed [this tutorial](https://www.geeksforgeeks.org/reading-and-writing-json-to-a-file-in-python/).

<br>

## Deliverable 2: Scrape and Analyze Mars Weather Data
<br>

### Step 1: Visit the Website
<br>

* Use automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html). Inspect the page to identify which elements to scrape.
<br><br>

### Step 2: Scrape the Table
<br>

* Create a Beautiful Soup object and use it to scrape the data in the HTML table.

* Note that this can also be achieved by using the Pandas `read_html` function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
<br><br>

### Step 3: Store the Data
<br>

* Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
<br>

    * `id`: the identification number of a single transmission from the Curiosity rover
    * `terrestrial_date`: the date on Earth
    * `sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    * `ls`: the solar longitude
    * `month`: the Martian month
    * `min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
    * `pressure`: The atmospheric pressure at Curiosity's location

<br>

### Step 4: Prepare Data for Analysis
<br>

* Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate `datetime`, `int`, or `float` data types.
<br><br>

### Step 5: Analyze the Data
<br>

* Analyze your dataset by using Pandas functions to answer the following questions:

    1. How many months exist on Mars?

    2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?

    3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:

        * Find the average the minimum daily temperature for all of the months.

        * Plot the results as a bar chart.

    4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:

        * Find the average the daily atmospheric pressure of all the months.

        * Plot the results as a bar chart.

    5. About how many terrestrial (Earth) days exist in a Martian year? To answer this question:

        * Consider how many days elapse on Earth in the time that Mars circles the Sun once.

        * Visually estimate the result by plotting the daily minimum temperature.

<br>

### Step 6: Save the Data
<br>

* Export the DataFrame to a CSV file.