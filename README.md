# PROJECT NAME, Saas and Enterprise companies in PHX, Arizona

# PROJECT SUMMARY:

Arizona's economy has evolved. 
Arizona historically used to run on the 5 "C"'s : Copper, Cotton, Cattle, Citris & Climate but the landscape has changed. 
Now, according to the Arizona Commerce and Department of Labor Arizona is now fueled by manufacturing in areospace, electronic, semiconductor and software. Playfully nicknamed the "Silicon Desert" Phoenix is definitly a growing tech hub. 
We wanted to choose datasets to work with that are current,relevant to us, and most importantly immediatly useable. 
Below is the documnetation for this project.

# Future Use Possibilty 
Eventually the idea is to build out this project into an exploratory career search tool where people can collect a list of company names to explore that are pf particular interest to that individual. This would be a tool for people who would like to find jobs based on industry, proximity, size and other non-traditional search perameters, characteristics like female CEO, type of software, etc.

Becuase this list beingn added to constantly we could create an API to check the site for new entries and write them to the existing DB, adding them as new options for the person to find. 



# ETL-Project - Group 1

# INTRODUCTION
# The two sources we extracted from


1.) SaaS Companies with offices in Phoenix, AZ that have female CEO 
https://gregslist.com/phoenix/software-companies-other/woman-ceo/



2.)  Gregslist of Software Companies in Phoenix, AZ  
https://gregslist.com/phoenix/


#Data Cleanup & Analysis, (See Jupyter notebook)

Took a long time extracting the data from the HTML. 
It was a very tricky thing and eventually we found that a look within one company at a time was the best way to accurately extract info without leaving missing spaces and messing up the order of extracted info. 
Here we took 3 major things: NAME, DETAILS,& WEBSITE from both the female CEO list as well as the Software company list and plan on joining them into a concise list. 
We anticipate there may be duplicates and we will clean those up using the the company NAME column. 

# 1.) Extract
Data was in HTML and we extracted it using web scraping techniques.
We extracted a portion of the page that houses the lsit and then narrowed it down to include the whole list from one page and then to one company.
You can see many of these in the notebook. We needed to grab the info based on the container in order not to set off the order of the information being scraped. This also showed us the advert block that shows an empty NAME and DETAILS line and only lists the sponsor for that section. 

# 2.) Transform
We cleaned and joined these csv's.
Join on company name, getting rid of duplicates and preserving the integrity of the data by doing a 
loop that allows us to see any missing values in the data scraped. Merged the two csv's into one list that encompasese the first page of SOFTWARE companties and all of the women CEO saas compaines. 

# 3.) Load
Loaded into one csv. This list is always expanding and this way we can keep adding to it.
 hopefully better understand and get more familiar with the tech landscape of Arizona and know where we might be a good fit. 
