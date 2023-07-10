# beautifulsoup_challenge

Background
--------
Extract information from the [Mars News Website](https://static.bc-edx.com/data/web/mars_news/index.html) and the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html) via both automated browsing with Splinter and HTML parsing with Beautiful Soup. Analyze the data extracted and save it to a CSV file. 

## Objective ##
#### Part 1: Scrape Titles and Preview Text from Mars News ####
- Use automated browsing to visit the [Mars News Website](https://static.bc-edx.com/data/web/mars_news/index.html). 
- Create a Beautiful Soup object and use it to extract text elements from the website.
- Extract the titles and preview text of the news articles that were scraped. Store the scraping results in Python data structures as follows:
  - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: `title` and `preview`.
  - Store all the dictionaries in a Python list.
  - Print the list in the notebook.
<img width="900" alt="Screenshot 2023-07-09 at 9 54 53 PM" src="https://github.com/m-janssens-boop/beautifulsoup_challenge/assets/127706155/df691b1f-b76a-4394-8567-28a3769cbb66">

#### Part 2: Scrape and Analyze Mars Weather Data ####
- Use automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html).
- Create a Beautiful Soup object and use it to scrape the data in the HTML table.
- Assemble the scraped data into a Pandas DataFrame, with the same column headins as appear on the website. Thay are as follows:
  - `id`: the identification number of a single transmission from the Curiosity rover
  - `terrestrial_date`: the date on Earth
  - `sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
  - `ls`: the solar longitude
  - `month`: the Martian month
  - `min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
  - `pressure`: The atmospheric pressure at Curiosity's location
- Convert datatypes to proper formats.
- Analyze the dataset using Pandas functions, answering the following questions:

  - How many months exist on Mars?
  - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
  - What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
  - Find the average minimum daily temperature for all of the months.
  - Plot the results as a bar chart.
<img width="579" alt="Screenshot 2023-07-09 at 9 56 23 PM" src="https://github.com/m-janssens-boop/beautifulsoup_challenge/assets/127706155/e3bdfb36-2412-47b1-a318-41f9aac56b6f">

  - Which months have the lowest and the highest atmospheric pressure on Mars? This is done by:
    - Finding the average daily atmospheric pressure of all the months.
    - Plotting the results as a bar chart.
  - About how many terrestrial (Earth) days exist in a Martian year? This is done by:
    - Considering how many days elapse on Earth in the time that Mars circles the Sun once.
    - Visually estimating the result by plotting the daily minimum temperature.
<img width="895" alt="Screenshot 2023-07-09 at 9 56 42 PM" src="https://github.com/m-janssens-boop/beautifulsoup_challenge/assets/127706155/3804791b-5435-4f4a-8d2d-6be6883dfcc0">

