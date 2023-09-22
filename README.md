# Identifing the Top 10 Countries globally that have the least Healthcare access
<br>

Doctors Go Anywhere are looking to expand their outreach after their recent funding. In order to understand where their services would be the most valuable, they would like to identify the Top 10 regions that have the lowest access to healthcare.
<br>
The objective of this project, alongside identifing the above, we will also be looking into the following statements:
<br>
1) Investigate how the money invested by the Government into healthcare correlates a countries position in the rankings
2) Investigate how the Life Expectancy correlates with a countries position
<br>
# Data Dictionary
<br>
The data used within this project was extracted from gapminder, the original csv files can be found within the data folder but can also be found at the following website: https://www.gapminder.org/data/
<br> <br>
To insure that the data is consistent and to accomdate for certain missing data we will be taking the data from 1995 to 2010 for all the selected datasets.
<br>
|Feature|Type|Dataset|Description|
|---|---|---|---|
|Population data set|  |  |
|country|*object*|Afganistan|Contains the name of all the countries|
|1995-2010|*float*|17800000.0|Columns containing the population per country ranging from 1995 to 2010|
| | | | |
|Life Expectancy data set|  |  |
|country|*object*|Afganistan|Contains the name of all the countries|
|1995-2010|*float*|81.1|Columns containing the Life expectancy per country ranging from 1995 to 2010|
| | | | |
|Health Aid data set|  |  |
|country|*object*|Afganistan|Contains the name of all the countries|
|1995-2010|*float*|97.40|Columns containing the amount of health aid provided per person by the country's government ranging from 1995 to 2010|
| | | | |
|Medical Doctors data set|  |  |
|country|*object*|Afganistan|Contains the name of all the countries|
|1995-2010|*float*|1.12|Columns containing the number of doctors per 1000 per country ranging from 1995 to 2010|
| | | | |
|Merged Population & Health Aid provided per Person|  |  |
|country|*object*|Afganistan|Contains the name of all the countries|
|1995-2010 Population|*float*|17800000.0|Columns containing the population per country ranging from 1995 to 2010|
|1995-2010 Health Aid|*float*|1.12|Columns containing the amount of health aid provided per person by the country's government ranging from 1995 to 2010|
<br>
# Executive Summary
<br>
Healthcare is probably one of the most discussed topics around, with places like the UK having their free healthcare and others having a well developed private healthcare system like the US and Australia. In this project we will be looking to identify the top 5 companies where majority have the least amount of access to healthcare support/doctors.
<br>
By identifying this list will allow us to better understand what countries would benefit from receiving external support. However, we don't want to just stop there, Doctors, just like the rest of us need to get paid, so how does the amount invested into the healthcare system (both public and private) affects a countries ranking position.
<br>
To expand on this we will also be looking at life expectancy from two different point of views. One point will be is that, naturally most of us would assume that countries that have the least amount of doctors will have the lower life expectancy, creating a graph with a negative correlation, but what does the data show. Could it be that the countries with the least amount of doctors and relying on other forms of healthcare or alternative medicine giving them a longer life.
<br>
Lastly we will also be looking at how it is affected by the amount of money that has been invested into the healthcare system. Once again most of us naturally would assume that the countries that have invested less into their healthcare have the lower life expectancy for their population, creating a graph with a negative correlation. However, what does the data show, as they may be countries that invested heavily into their healthcare system to improve and develop it but still have a low life expectancy.
<br>
Explain why I dropped 2020-2023 in the life expectancy data
<br>
# Methodology
<br>
To identify the Top 10 countries we will be talking the population and number of doctors per 1000 data found on gapminder to identify the countries that have the least amount of doctors. The population of the countries must be considered to ensure a fair comparison is made. For example if both Country A and B have 10,000 doctors but A has a population 1 million and B has 4 million. Which means from first impressions you would have thought, they were the same but when you bring population into the equation we can see that country B would higher in the ranking for least accessible healthcare system.
<br><br>
In order to do this, I will be calculating the taking the average number of doctors for each country, to accomdate for any missing data from across the years. The missing date could be due to a number of things such as, the governments not having the resources or not having the money to consistently collect the data or many other reasons. To ensure that data wasn't simply dropped and missing out on countries that could potentially be at the top of the list an average will be calculated. Where there is only 1 data point, the assumption will be made that the number has stayed constant.
<br><br>
When looking into the money invested into healthcare we looking at the amount of money the government has on average spent per a person. We will be taking that data and multiplying it by the population and then calculating the mean in order to understand how much each country has invested into their healthcare industry over the last 10 years. This will be plotted against 
<br>
# Conclusion & Recommendations
<br>
In conclusion we identified the following list which shows the Top 10 countries that have the least amount of doctors that could potentially benefit from receiving additional funding.
<br>
|Ranking Position|Lowest amount of Doctors Country|Lowest amount of money spent Country|Lowest Average Life
|---|---|---|---|
| 1 | Ukraine | Ukraine  | Eritrea |
| 2 | Naura | Naura | Kiribati |
| 3 | Slovenia | Slovenia | Nauru |
| 4 | Gambia | Gambia | Gambia |
| 5 | Colombia | Colombia | Sao Tome and Principe |
| 6 | Kiribati | Kiribati | Ukraine |
| 7 | Sao Tome and Principe | Sao Tome and Principe | Egypt |
| 8 | Turkey | Turkey | St. Kitts and Nevis |
| 9 | St. Kitts and Nevis | St. Kitts and Nevis | Brazil |
| 10 | Egypt | Egypt | China |
<br>
From the list above we can make the assumption that on average the less a country spends on their populations healthcare, the less doctors that population will have access to. Now this is still as they could be other factors involved for example the education system not being developed enough.
<br>
When comparing the average life expectancy to the lowest amount of doctors we can see that the list has changed up. With 3 new location popping up; Eritrea, China and Brazil. This raises an interesting question as all 3 where found in the Top 10 highest healthcare contribution by the government as you can see from the list below. As a recommendation I would suggest to look further into why this could potentially be the case.
<br>
I would also recommend find data regarding private healthcare to see how it could potentially change these finding as many countries do rely more on the private services that are available.
<br>
|Ranking Position|Highest Healthcare Contribution Countries|
|---|---|
|1| Japan |
|2| Czech Republic|
|3| Fiji|
|4| Italy|
|5| Canada|
|6| Eritea|
|7| China|
|8| Netherlands|
|9| Austrialia|
|10| Brazil|
<br>
Some more recommendation that can be made from my findings are list below:
1) Understand how China a significantly large amount of Doctors whilst having a low amount of contribution from the government
2) Investigate Why China and San Marino took a deep in life expectancy from 1995 to 2002
3) Investigate how Japan has one of highest life expectancies with a low amount of Doctors compared to the rest.