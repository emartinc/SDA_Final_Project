---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "Is It Just Bad Driving - or is the Weather to Blame?"
subtitle:  "Exploring the Link Between Weather and Traffic Accidents: A Data-Driven Study in NYC"

---

Every year, an estimated 1.19 million people lose their lives in road traffic accidents, while another 20 to 50 million suffer non-fatal injuries. Many of them resulting in long-term disabilities [1]. But what exactly is a traffic accident? At its core, it is an unplanned event that occurs in a specific time and place, often involving one or more vehicles, leading to physical harm. Understanding with data when and where these incidents happen is key to grasping the causes and patterns. 

From a young age, we’re taught the golden rules of safe driving: don’t drink and drive, obey speed limits and avoid getting behind the wheel during bad weather. But how much truth is there to that las piece of advice? Is it really unsafe to drive in the rain or snow, or do we just assume it is? And when an accident happens, who or what is truly at fault? Is it human error: speeding, distraction, poor decisions, bad infrastructures, or does the weather itself play a more significant role than we think?

To explore these questions, we’ll take a closer look at traffic accidents in New York City and their relationship with weather conditions. The goal is to understand whether these incidents are primarily dirven by human factors or significantly influenced by external forces like the weather. New York is an ideal case study. It experiences a wide range of weather conditions, from heavy snowfall in winter to hot, humid summers. Combined with its dense population and fast-paced urban life, the city provides a rich dataset that allows us to examine both environmental and human variables in a complex, high-pressure setting. Its chaotic and highly populated nature makes it the pefect environment to observe how weather and human behavior intersect on the road. 

## Are We Getting Safer? A Look at the Accident Trends.

<figure class="figure-wrapper">
  <img src="{{ site.baseurl }}/assets/images/accidents_per_year.png" alt="Accidents Per Year">
  <figcaption class="figure-caption">Figure 1: Traffic Accidents per year spanning from 2012 to 2024.</figcaption>
</figure>

When looking at traffic accidents by year, 2017 clearly stands out as the peak, recording the highest number of incidents. From 2012 to 2017, the number of traffic accidents increased, with its highest point in 2017. After that peak, the numbers begin to decline, with a small  drop in 2018 and 2019. Then, in 2020 there is a noticeable decrease, likely influenced by the COVID-19 pandemic and related lockdowns, which heavily influenced urban mobility. From 2021 to 2024, accident numbers continued to fall, though at a more stable rate, reaching similar levels to 2012. The change of traffic accidents from 2021 to 2024 is probably influenced by commuting behavior, remote work, and fewer vehicles on the road due to the pandemic. 

## A Curious Disconnect: Fewer Accidents, More Fatalities?

<figure class="figure-wrapper">
  <iframe src="{{ site.baseurl }}/assets/images/deaths_per_year.html" width="100%" height="500" frameborder="0"></iframe>
  <figcaption class="figure-caption">Figure 2: Fatalities per year (2012 - 2024)</figcaption>
</figure>

When looking at traffic fatalities by year, 2017 stands out with a notably high number of deaths, reinforcing its relevance as a key year for analysis. Interestingly, there are also spikes in fatalities in 2013 and during the pandemic years, particularly between 2021 and 2023, despite the fact that the total number of accidents was significantly lower during that period. In 2024, fatalities drop slightly, but the decrease is minimal. 

This mismatch between accident frequency and fatal outcomes suggests that fewer accidents don’t necessarily means safer roads. It raises important questions: Could it be due to the severity of crashes? Changes in driver behavior, or even factors like vehicle design, road infrastructure or emergency response times? While 2017 had the highest number of accidents and remains a data-rich year, the lack of direct correlation between accident volume and fatalities hint a deeper, more complex causes to explore. 


## Where Accidents Happen: A Geographic Breakdown of NYC Boroughs.

To better understand where accidents are most concentrated within the city, we turn to a borough-level analysis for the years 2017–2018. The spatial distribution of incidents reveals striking differences across New York’s five boroughs, shedding light on how geography, infrastructure, and population dynamics shape road safety.

<figure class="figure-wrapper">
  <iframe 
  src="{{ site.baseurl }}/assets/images/accidents_borough_fixed.html" 
  width="100%" 
  height="650" 
  style="border:none; display:block; margin:0 auto;">
</iframe>


The map presents a clear spatial distribution of traffic accidents across New York City's boroughs between 2017 and 2018. Unsurprisingly, Brooklyn and Queens exhibit the darkest shades, indicating the highest number of traffic accidents, likely reflecting their larger populations, greater roadway networks, and high vehicle ownership. Despite its smaller size, Manhattan also shows a high accident count, possibly due to dense traffic volumes, tourism, and a high rate of pedestrian activity.

In contrast, Staten Island and the Bronx recorded significantly fewer accidents, with Staten Island having the lowest count, consistent with its lower population density and more suburban layout. This geographical trend underscores how urban density, transportation habits, and borough-specific infrastructure can influence traffic safety outcomes.

## When Accidents Happen: Analyzing Hourly Trends in Traffic Accidents.

<figure class="figure-wrapper">
  <iframe src="{{ site.baseurl }}/assets/images/accidents_by_hour_polar.html" width="100%" height="800" frameborder="0"></iframe>
  <figcaption class="figure-caption">Figure 4: Accidents per hour of the day, year 2017</figcaption>
</figure>

When analyzing traffic accidents by hour of the day across NYC boroughs: Bronx, Brooklyn, Manhattan, Queens and Staten Island, a consistent daily pattern emerges. Accidents are most frequent between noon and 6 PM, likely reflecting the combined effects of midday traffic and afternoon rush hour. After 6 PM there a slight dip, but interestingly, a noticeable spike occurs again around 9 PM. Following that, the number of accidents drops significantly between 10 PM and 5 AM, where the road activity is generally lower. At 6 AM, there is a noticeable spike, possibly linked to early commuters, though the pattern briefly dips again at 7AM before rising once more as the day progresses. 

Several interesing patterns emerge from this graph. The notable peak around 3 PM and 4 PM may correspond to school dismissals and afternoon traffic congestion. On the other hand, the lowest number of incidents occurs between 1 AM and 5 AM, likely due to minimal traffic volume. However, the accidents that do happen during these hours could be related to driver fatigue, alcohol consumption or poor visibility. This suggests that while collisions are less frequent overnight, they may be more severe or fatal due to the risky conditions in which they happen since alcohol consumption is one of the main causes of traffic fatalities [1].

What stands out is the consistency of this hourly pattern across all boroughs, suggesting that time of day plays a more significant role in predicting accident frequency that geographic location alone. While some boroughs report more accidents overall, likely due to higher population density or traffic flow, this shared temporal rhythm implies a strong behavioral influence. 

Additionally, the unexpected spike around 9 PM could be linked to post-dinner activities, outings, events or nighttime driving routines. Insights like these are valuable for resource planning and public safety strategies, such as increasing patrol presence during high-risk hours or launching targeted awareness campaigns during the evening peak. 

## A Year of Weather in NYC: Setting the Scene for Traffic Analysis

<figure class="figure-wrapper">
  <img src="{{ site.baseurl }}/assets/images/average_temp_month.png" alt="Accidents Per Year">
  <figcaption class="figure-caption">Figure 5: .</figcaption>
</figure>

The climate in New York throughout 2017 and 2018 shows clear seasonal variation. Temperatures are highest from June to September, with July and August reaching peak averages of 25.1ºC and 24.5ºC, respectively. On the other end, the coldest months fall between December and March, with January averaging as low as 0.5ºC. The transitional months, April, May, October and November, present moderate temperatures. 

<figure class="figure-wrapper">
  <img src="{{ site.baseurl }}/assets/images/precipitation_month.png" alt="Accidents Per Year">
  <figcaption class="figure-caption">Figure 6: .</figcaption>
</figure>

In terms of precipitation, March stands out as the month with most snow, followed by January and February, making the core of winter. There’s also a peak in snowfall in November and December, indicating the onset of colder conditions. During the summer months and the months prior and after it, snowfall drops to zero. 
When it comes to rainfall, July and August are the rainiest months alongside May, which also sees a high level of precipitation. Interestingly, June is one of the driest months, just before precipitation peaks in midsummer. Overall, NYC experiences a full range of weather conditions throughout the year, making it an ideal setting to explore how temperature and precipitation may impact traffic accidents. 

## Uncovering the Truth: What Effect Does Weather Have On Traffic Accidents?  
The relationship between weather conditions and traffic accidents in New York during 2017 does not reveal any strong or direct correlations. While it is common to assume that poor weather increases the likelihood of accidents, the data suggests a complex reality influenced by seasonal patterns and human behavior. 

<figure class="figure-wrapper">
  <img src="{{ site.baseurl }}/assets/images/comparison.png" alt="Accidents Per Year">
  <figcaption class="figure-caption">Figure 7: .</figcaption>
</figure>

In terms of temperature, there is no clear link between warmer and colder months and the number of accidents. Although the highest temperatures occur in July and August, accident rates are relatively low during these months. In contrast, May and June, which mark the start of the warmer season, show the highest accident rates. This might be due to increase activity or traffic density before summer holidays begin, but overall, temperature alone does not appear to be a strong predictor of accidents. 


Regarding precipitation, there is some alignment during the early months of the year. February, March and April have their levels of precipitation matching with the number of accidents. The peak in March could be linked to it being the month with most snow, thus, having a relationship with more accidents. However, this pattern does not hold throughout the year. For example, July, one of the driest months, still shows elevated accident levels, suggesting that rainfall may influence risk, but only in combination with other factors.

With cloud coverage, there is a more consistent pattern. Months with lower cloud cover, such as June and July, have higher accident rates. This could indicate that clearer skies invite more driving, faster speeds or lower perceived risk, potentially leading to more accidents.

Concerning wind speed, a similar inverse relationship is observed. Months with higher average wind speeds, such as March and April tend to have fewer accidents, while calmer months like May and June coincide with more accidents. One possible explanation is that adverse wind conditions may make drivers more cautious or reduce overall traffic volume.

Overall, while none of the weather variables alone can fully explain the fluctuations in accident rates, their interaction with human behavior, including travel patterns, perceived road safety and seasonal routines, likely plays a critical role.




---
