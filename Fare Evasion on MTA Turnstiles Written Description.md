# Fare Evasion in New York MTA Turnstiles


##### Abstract
The main goal of this project is to minimize the rate of fare evasion crime in New York City through the betterment of distribution of the manpower of NYPD (New York Police Department) in the busiest stations since this study depicts a clear correlation between traffic and the possibility of fare evasion crimes happening in said stations. Moving over, provided with the data are graphs depicting trends, demographics which visualize the data points used which communicate the main purpose of this study.

##### Design
New York City suffered from fare evasion crime for so many years and the New York Police Department kept a record for the number of crimes happening on a yearly basis. The last recorded data was back in 2018. With the conjuction of the turnstile dataset from the same time period it resulted in useful insights ranging from the number of crimes per station all the way to the age group responsiable for fare evasion crimes.

##### Data
Two datasets have been used. The first one is the turnstile dataset which contains around 10M rows and 11 columns. Most notable columns include: entries, stations, C/A, unit and scp. The second dataset is the arrests for fare evasion crime from NYPD website. It contains 195,888 rows and 17 columns. The most critical columns in this dataset are: station, perp gender, perp age group, perp race and other more.


##### Algorithms
 Exploratory Data Analysis was done to both datasets.
 
 **MTA Turnstile Dataset:**
  - Cleaning: duplicated values were eliminated alongside irregular and false readings. Outliers were also discarded. Additional whitespaces were removed from columns. Lastly the focus was drawn to the entries only since fare evasion occurs in the entrances. With that being said, the unneccessary columns were dropped like: exits, linename, division and describtion.
  
  - Exploring: the data was explored by performing the correlation and the covariance calculations to establish a relationship between the two datasets.
  - Aggregating: the use of (group by) was heavy in both python and in sqlAlchemy to prepare some dataframes to visualizing and to also merge multiple dataframes.
  - Visualizing: various graphs were done to determine the top 10 busiest stations and the daily entries throughtout the year of 2018 either per week or for the whole time period.

 **Arrests Turnstile Dataset:**
  - Cleaning: unneccessary columns were dropped like: objectid, arrest key, jurisdiction code and arrest precint, line and many more.
  
  - Exploring: like the MTA dataset the data was explored by performing the correlation and the covariance calculations to establish a relationship between the two datasets.
  - Aggregating: (group by) was used to count the number of crimes for each station and to add more features to the resulting dataframe for example: the age group who are responsible for fare evasion crime in each station
  - Visualizing:  graphs were drawn to figure out the top 10 heavy crime stations with more features to help in providing useful insights like: age, gender, district and race.

##### Tools
1. Numpy
2. Pandas
3. Matplotlib
4. Seaborn
5. SqlAlchemy
6. Jupyter



