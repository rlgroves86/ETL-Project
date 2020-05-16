# ETL-Project - Group 1

 ###Finding Data
#The two sources we extracted from


1.) SaaS Companies with offices in Phoenix, AZ that have female CEO 
https://gregslist.com/phoenix/software-companies-other/woman-ceo/



2.)  Gregslist of Software Companies in Phoenix, AZ  
https://gregslist.com/phoenix/


### Data Cleanup & Analysis
#See Jupiter notebook
Took a long time extracting the data from the HTML. It was a very tricky thing and eventually we found that a look within one company at a time was the best way to accurately extract info without leaving missing spaces and messing up the order of extracted info. 
Here we took 3 major things: NAME, DETAILS,& WEBSITE from both the female CEO list as well as the Software company list and plan on joining them into a concise list. We anticipate there may be duplicates and we will clean those up using the the company NAME column. 

#Extract
Data was in HTML and we extracted it using web scraping techniques.
YOu can see many of these in the notebook.

#Transform
We cleaned and joined these lists.See Jupiter notebook.
Join on company name,getting rid of duplicates and preserving the integrity of the data by doing a 
loop that allows us to see any missing values in the data scraped.Questions, Ask.

#Load
Loaded into CSV and then into tables in mongoDB.
This list is always expanding and this way we can keep adding to it.
Also loaded in DF so we can see it and hopefully better understand and get more familiar with the tech landscape of Arizona and know where we might be a good fit. 
