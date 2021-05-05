
# COVID Testing in US v. South Korea

## Executive Summary
I wanted to see how the United States fared in COVID-19 testing compared to a nation that was regarded as vigorously testing.   South Korea was testing daily since February 2020, the United States was slow to ramp up testing capacity in compariosn.  This project is an attempt to see how far behind the curve we were compared to South Korea.

## Data
Data was pulled from  [US](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/testing-in-us.html) and [South Korea](https://www.cdc.go.kr/board/board.es?bid=0030&mid=) CDC pages between February 8 and March 15 2020. For the US data, I used Python and BeautifulSoup to scrape the data from HTML tables. For the South Korea information, data was manually inputed from the press release pages. The press release format differed each day, so was unable to use a web scraper.

## Visualizations

### Daily testing in US v. South Korea
![Daily testing](/plots/daily_testing.png)
Web scraping was done in Python [here](/code/001_data_collection.ipynb) and visual was made in D3.js [here](/code/index.html)

As of March 15, the US had only tested 0.00097% of its total population. With all the efforts to shelter in, how do we know if we are "flattening the curve" when we don't know the true value of the curve?
![US test v. cases](/plots/US_test_cases.png)

### Daily testing in US by State
![State testing](/plots/state_testing.png)
Data source is from [The COVID Tracking Project](https://covidtracking.com/data/), and visual was made with R Shiny [here](/code/plotly_shiny)

## Next Steps
I would like to update my code to pull the data automatically daily, so the dashboard will be updated. I would also like to include information and resources for WHERE to get testing in your state/region.
