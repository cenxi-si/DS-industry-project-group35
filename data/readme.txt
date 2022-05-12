JOINING FILE
'Code.RDS' contains a list of all of the fbi departments, their office identifier (ORI), and the county, city, and cbsa associated with the department.
This file helps match data from various sources with different identifiers.
County, city, and cbsa are different geographic units in America. Note that some ORIs are associated with multiple geographic units (e.g., one FBI office collects data on multiple cities within its jurisdiction)
Nore that 'Code.RDS' is a file I created. The US Census Bureau has their own 'delineation_file', which lists which cities/counties fall within certain CBSAs. Their version does not contain the FBI ORI codes, though, as the census bureau and fbi are separate entities.

ALCOHOL DATA
from data.census.gov
Example for year 2016:
https://data.census.gov/cedsci/table?text=CB1600CBP&g=0100000US%240500000,%243100000&y=2016&n=445310&tid=CBP2016.CB1600CBP&nkd=EMPSZES~001
CB1600CBP - alcohol outlets in each county for year 2016...
To find data for 2017 for example, search for table CB1700CBP.
Note NAICS code for alcohol = 445310
Data is only available yearly
There are multiple geographic options available. Metro and micropolitan statistical area refers to CBSA (I'm pretty sure...but double check)
I have alcohol data from 2012 to 2016 at the cbsa level, but the rest will need to be collected.

CRIME DATA
The crime data was downloaded from the University of Michigan. Example for 2016: https://www.icpsr.umich.edu/web/NACJD/studies/37057
The data is available monthly. I have the data from 2012 - 2016, but the rest will need to be collected.
The files are called "Uniform Crime Reporting Program Data; Arrests by Age,Sex, Race, United States YEAR"
There is one file for each year available. I have data for 2012-2016, its in this file called "crimeall.RDS"
There is a codebook for each year, which downloads as a pdf when you download the data.
Note that there were naming convention changes between crime data collected in 2012/13/14/15 versus 2016. in crimeall.RDS, I merged the files correctly and in some cases by renaming variables manually, so all variables mapped correctly. To see these differences, you need to look at the codebooks for the different years.
There may be naming change conventions from these data to data from 2017/2018/2019/2020/2021. Be ware.
Offense = "20 " is 'offenses against family and children'. This is what we used to operationalize 'domestic violence' crimes.
There are other offenses, too. Check out the codebook.


TWEET DATA
I'll need to process this again, and gather the data for all the years
Tweet data is available with a timestamp so can be aggregated to the month, to match crime data.
Tweets are geolocated at the US city level, which can then be merged with crime data.
In "tweets.RDS" I've included the last lot of twitter data, which contains 2013/2014/2015 tweets on misogyny. If desired, you could use this to start approximating the data, but note that this is not the final data, only a rough indication of the data. It will take a few weeks to get this data from Twitplat. 


THE FOLDER CENSUS DATA
Contains relevant predictors of domestic violence at the geographic level. Note, however, that data is only available yearly.
Hence I don't think this will be relevant for our analyses.