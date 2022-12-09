Infectious Disease Outbreaks on Twitter 

----------------------------------------------------- 

1. Introduction 

This dataset contains tweets referencing infectious disease outbreaks in the U.S. after the official announced date on the CDC website (https://www.cdc.gov/outbreaks/index.html). Each set of tweets related to a disease outbreak was output to a csv file and a total_tweet.csv file was created that contains the total number of tweets returned for each disease. 
Government disease agencies or epidemiologists could compare the number of tweets about different outbreaks generated in this project to gauge public awareness of each outbreak and potentially track new disease outbreaks. 

2. Description 

This project uses BeautifulSoup to get the list of current outbreaks from the CDC website. Then snscrape is used to query for tweets mentioning each disease outbreak from Twitter. The tweets are put into a pandas dataframe, then converted into a csv file.  
Each disease outbreak csv file contains the following columns: 

Tweet_ID: the ID of the tweet 
Date: the date when the tweet was generated 
User_ID: the ID of the Twitter user who generated the tweet 
Location: the location of the Twitter user 

Due to Twitter term restrictions, the full tweet content will not be shared.  

----------------------------------------------------- 

The following is a summary of the csv files for the disease outbreaks that are currently listed on the CDC website. While this project limited the maximum number of returned tweets to 1000 for each disease outbreak, the limit of tweets returned could be raised in the tweet_search function’s limit variable.  

File: total_tweet.csv 
Description: name of each outbreak and the number of tweets of each outbreak 
Size: 402 bytes  
Format: First row is the outbreak name. Second row is the number of tweets. 

File: enoki mushroom listeria.csv 
Description: Tweet’s about listeria outbreak linked to enoki mushrooms 
Size: 193 tweets 
Format: Each file contains the following columns: Tweet_ID, Date, User_ID, Location 

File: listeria deli meat.csv 
Description: Tweet’s about listeria outbreak linked to deli meat and cheese  
Size: 935 tweets 
Format: same as enoki mushroom listeria.csv 

File: salmonella fish.csv 
Description: Tweet’s about salmonella outbreak linked to fish 
Size: 148 tweets 
Format: same as enoki mushroom listeria.csv 

File: salmonella bearded dragons.csv 
Description: Tweet’s about salmonella outbreak linked to bearded dragons 
Size: 75 tweets 
Format: same as enoki mushroom listeria.csv 

File: E. coli frozen falafel.csv 
Description: Tweet’s about e. coli outbreak linked to frozen falafel 
Size: 251 tweets 
Format: same as enoki mushroom listeria.csv 

File: listeria Brie Camembert cheese.csv 
Description: Tweet’s about listeria outbreak linked to brie and camembert cheese 
Size: 252 tweets 
Format: same as enoki mushroom listeria.csv 

File: salmonella turtles.csv 
Description: Tweet’s about salmonella outbreak linked to fish 
Size: 653 tweets 
Format: same as enoki mushroom listeria.csv 

File: hepatitis children.csv 
Description: Tweet’s about hepatites of unknown cause in children 
Size: 1000 tweets 
Format: same as enoki mushroom listeria.csv 

File: coronavirus COVID-19.csv 
Description: Tweet’s about Coronavirus 
Size: 1000 tweets 
Format: same as enoki mushroom listeria.csv 

File: lung injury e-cigarette vaping.csv 
Description: Tweet’s about lung injury associated with e-cigarette use or vaping 
Size: 1000 tweets 
Format: same as enoki mushroom listeria.csv 

File: raw milk brucella.csv 
Description: Tweet’s about brucella caused by containing raw milk 
Size: 367 tweets 
Format: same as enoki mushroom listeria.csv 
 
File: measles.csv 
Description: Tweet’s about measles outbreak 
Size: 1000 tweets 
Format: same as enoki mushroom listeria.csv 

File: hepatitis A homeless.csv 
Description: Tweet’s about outbreaks of hepatitis a in multiple states among people who are homeless 
Size: 1000 tweets 
Format: same as enoki mushroom listeria.csv 

File: monkeypox.csv 
Description: Tweet’s about Monkeypox  
Size: 1000 tweets 
Format: same as enoki mushroom listeria.csv 

File: ebola congo 2018.csv 
Description: Tweet’s about Ebola in Congo in 2018 
Size: 1000 tweets 
Format: same as enoki mushroom listeria.csv 
 
File: ebola congo 2017.csv 
Description: Tweet’s about Ebola in Congo in 2017 
Size: 366 tweets 
Format: same as enoki mushroom listeria.csv 

----------------------------------------------------- 

3. Installation  

There are some general library requirements for the project and some which are specific to individual methods. The general requirements are as follows: 

BeautifulSoup 
datetime 
Pandas 
pprint 
requests 
snscrape 

Please note, snscrape requires installation of Python 3.8 or greater. 

4. Access Rights and Mode of Distribution 
 
The csv output files are provided directly to users of this application. This project, and all data contained within, are considered open source for academic, research, and personal use and will be made publicly available. 

5. Limitations 

Each user's location is free-text and not a required field on Twitter. We opted to include location for each tweet as a field in the dataset, but acknowledge that this data may be both limited and unreliable. 
We chose to omit the actual tweet content and to only include IDs for the original posts to allow for reproducibility of the dataset construction and to be compliant with Twitter data access rights. 
We manually wrote each query based on the output from our scrape of the CDC website. However, in the future, we would like to build some kind of natural language processing tool to read the name of each outbreak and find meaningful queries with which to search Twitter, and perhaps to create multiple queries for each outbreak to capture all keywords. 
Pandas is not always the correct tool for large datasets that do not fit into a user's local memory. In further development of this project, we will need to move to another tool to fit the needs of a larger dataset.  

6. Authors 

Hong Doan 
Alex Hoang 
Anh Nguyen 
Morgan Purcell 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 