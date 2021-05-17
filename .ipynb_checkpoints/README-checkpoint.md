# US Stock market vs Cryptocurrency trend analysis

## Including the trend comparison before and during the COVID-19 Pandemic (using 2020-1-1 as this incident's separator)

This data analysis project compares the trend of US Stock market and Cryptocurrency market throughout 2016-04-01 till 2021-3-31, for the sake to analyze whether two markets correlates (or inversely correlates) with each other, and how COVID-19 Pandemic changes such correlation. Bitcoin and other cryptocurrencies have become a more and more popular alternative investment vehicle (than the US Stock market), especially during the COVID-19 pandemic that has brought Bitcoin's price from $6000 to $6000**0** at one point. Result from this data analysis can inform readers how similar (or different) does the US Stock market and Cryptocurrency market behave, which might provide them useful information when they're investing in either market.

## Dataset Used

* Daily Value of Dow Jones Industrial Average index (DJIA) (The final project uses data dated 2011-05-16 to 2021-05-14)
* Daily Value of Standard & Poors 500 index (S&P 500) (The final project uses data dated 2011-05-16 to 2021-05-14)
* Daily Price for Bitcoin in US Dollar (The final project uses data dated 2010-07-18 to 2021-04-25)
* Daily Price for Ethereum in US Dollar (The final project uses data dated 2016-03-10 to 2021-04-25)


## Steps to fetch DJIA and S&P 500 dataset .csv files

Visit [this DJIA dataset source](https://fred.stlouisfed.org/series/DJIA) and [this S&P 500 dataset source](https://fred.stlouisfed.org/series/SP500). In the upper right corner there's an orange *edit graph* button, on the left of this button, there's a date picker. Choose the start date to a value as early as possible, then there's a download button where you can download .csv files. Place these two .csv files in the ./data/ folder so the Jupyter notebook can find them.

Unfortunately, datasets of DJIA and S&P 500's daily values can't be included in this GitHub repository since I need to obtain permission in order to re-distribute these two datasets.