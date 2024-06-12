# Greater Vancouver Housing Market Analysis

## The purpose of this project is to gather insight on the current Vancouver housing market utilizing Python for analysis and Tableau for visualization. <br/>

This is a full end to end data analysis project using data that has been webscraped from Zillow.com to derive the current housing market in the Greater Vancouver area. The core components of this project includes:
* Data scraping using python libraries such as beautifulsoup from Zillow.com
* Cleaning and transforming the data gathered from Zillow to ensure quality of data is consistent
* Exploratory data analysis to understand how key features affect the price that has obtained from the dataset such as number of bedrooms, square footage, and location
* Develop an interactive dashboard with all relevant information using Tableau (https://public.tableau.com/app/profile/victor.yung/vizzes)

Data Scraping
---
The current data collected for this project was obtained from Zillow.com with a focus on the Greater Vancouver Area. The python libraries utilized for this process includes beautifulsoup, json, and re. Locating the correct data within the website posed as a slight challenge as the relevation information such as square footage, number of bedrooms, number of bathrooms, unit type, and price were conglomerated into a html class called ''StyledPropertyCardDataArea-c11n-8-100-4__sc-10i1r6-0 dKKiyn property-card-link'. After finding the correct html class, I iterated through the pages using a for loop and appended the necessary details within the pages in a dataframe that was exported to a csv file.


Data Preprocessing
---
Once the data was collected, cleaning and transforming the data was necessary to ensure the quality was suitable for the analysis.
1. Changing column types to appropriate class.
2. Split various details from Housing Detail column into number of bed rooms, number of bathrooms, and square footage.
3. Trim and removed unnecssary characters from columns using lambda and regex functions.
4. Use pandas library pgeocode to convert postal codes into longitude and latitude.


Exploratory Data Analysis
---
Utilzied the correlation between three main features such as square footage, number of bedrooms, and number of bathsrooms to gain a better understanding of how sales price would be affected. Highest correlated feature would be square footage at 0.76 followed by number of bathrooms at 0.55 and lastly number of bedrooms at 0.34.

Moreover, the sales distribution is right skewed indicating the higher frequency of houses cover a wider range in the market for lower and less expensive homes.
<img width="915" alt="Screen Shot 2024-06-12 at 2 33 56 PM" src="https://github.com/vyung1996/Greater-Vancouver-Housing-Market/assets/132099834/07b2c4d3-966f-4a7f-b8d0-8ed67e4fe023">

We also notice the that Vancouver has generated the highest number of homes for sales. This is due to the population density of the area compared to the other cities. 
<img width="887" alt="Screen Shot 2024-06-12 at 2 34 29 PM" src="https://github.com/vyung1996/Greater-Vancouver-Housing-Market/assets/132099834/ebaba76d-c63f-4f11-94b6-5e5357897878">

Lastly, we notice that there is a positive linear relation between sales price and square footage. 
<img width="892" alt="Screen Shot 2024-06-12 at 2 34 16 PM" src="https://github.com/vyung1996/Greater-Vancouver-Housing-Market/assets/132099834/3b59c982-9625-415f-b0f8-571702260288">





