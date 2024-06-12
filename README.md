# Greater Vancouver Housing Market Analysis

## The purpose of this project is to gather insight on the current Vancouver housing market utilizing Python for analysis and Tableau for visualization. <br/>

This is a full end to end data analysis project using data that has been webscraped from Zillow.com to derive the current housing market in the Greater Vancouver area. The core components of this project includes:
* Data scraping using python libraries such as beautifulsoup from Zillow.com
* Cleaning and transforming the data gathered from Zillow to ensure quality of data is consistent
* Exploratory data analysis to understand how key features affect the price that has obtained from the dataset such as number of bedrooms, square footage, and location
* Develop an interactive dashboard with all relevant information using Tableau (https://public.tableau.com/app/profile/victor.yung/vizzes)

Data Scraping
---
The current data collected for this project was obtained from Zillow.com with a focus on the Greater Vancouver Area. The python libraries utilized for this process includes beautifulsoup, json, and re. Locating the correct data within the website posed as a slight challenge as the relevation information such as square footage, number of bedrooms, number of bathrooms, unit type, and price were conglomerated into a html class called ''StyledPropertyCardDataArea-c11n-8-100-4__sc-10i1r6-0 dKKiyn property-card-link'. After finding the correct html class, I iterated through the pages using a for loop and appended the necessary details within the pages in a dataframe that was be exported to a csv file.


Data Preprocessing
---
Once the data was collected, cleaning and transforming the data was necessary to ensure the quality of the analysis. 
