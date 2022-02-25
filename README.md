# surfs_up

## Introduction

you come up with a great idea for a new business, a surf & shake shop. You build a business plan which impresses W. Avey, a well know investor who is into surfing. While Mr. Avey was impressed with your presentation, he did some reservations. In a previous business deal, Mr. Avey had invested in a surf shop, but had not done any research into the weather conditions of the area where the shop was located. The shop was in a very rainy region and was rained out of business very quickly. Mr. Avey would like to not repeat that mistake with you and your new business, so he has asked you to do some research into the weather patterns of the area you want to build your new business.

He supplies you with a data file of weather reading from the area where you want to build the new business. The data file contains the following data points:

- Weather station reporting the data point
- The date of the reading
- The amount of precipitation on the date
- temperature observation on the date

When we look at the data file we see the following:

<img src="Resources\hawaii_data.png">

## Data Analysis

Mr. Avey asked us to analyze the weather pattern data for June and December to get an idea of what visitors to the area would expect to encounter if they came to surf.

The first step of our analysis is to read i the weather data and build dataframe. After reading in the date and temperature fields from the data file, we realize that the date is being read in as a string, so the next step in the analysis is to cast the date field as a datetime.

The next step in the analysis is to build a new column in the dataframe. This new column will be based on a calculation to determine the month of the weather reading.

<img src="Resources\load_data.png">

> An example would be 2010-01-01 would produce a month value of 1 for January.

<img src="Resources\temp_df_head.png">

Once the month column is calculated and filled, we can do the rest of the analysis that Mr. Avey requested. 

The first month he asked us to analyze was June throughout the years. So we look at the month column where month = 6. Once we have identified the dataset of weather data readings we can then do the summary statistics on the dataset for Mr. Avey.

<img src="Resources\june_results.png">

The second month Mr. Avey asked us to analyze was December throughout the years. So we look at the month column where month = 12. Once we have identified the dataset of weather data readings we can then do the summary statistics on the dataset for Mr. Avey.

<img src="Resources\dec_results.png">

## Summary

The analysis showed that the weather in Hawaii is wonderful.

The morning lows, afternoon highs, and overall average temperatures for both June and December are very similar. The obvious thing that the analysis shows is that December is a little cooler as it is winter time.

<table>
<tr>
<th></th>
<th>June</th>
<th>December</th>
</tr>
<tr>
<td>Min Temp</td>
<td>64</td>
<td>56</td>
</tr>
<tr>
<td>Max Temp</td>
<td>85</td>
<td>83</td>
</tr>
<tr>
<td>Avg Temp</td>
<td>75</td>
<td>71</td>
</tr>
</table>

Mr. Avey found our analysis very helpful and encouraging, he was still a little uneasy about investing. He said two more queries should be produced from the data set he gave us.

- The first is a similar analysis of the amount of precipitation for the months of June and December
- The second would be an analysis of of wave size for June and December 

