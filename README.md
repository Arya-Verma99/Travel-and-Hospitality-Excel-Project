# Travel & Hospitality : Navigating the Complexities of Airline and Airport Operations
## Objective 
The primary objective of this case study, titled "Sky Analytics: Navigating the Complexities of Airline and Airport Operations," is to deeply analyze and interpret the extensive datasets encompassing flights, airlines, and airports - namely "flights.csv", "airlines.csv", and "airports.csv". The analysis aims to uncover critical insights into flight operations, delay patterns, airline efficiency, and airport traffic dynamics. By exploring these datasets, the study seeks to identify key factors influencing operational efficiency, understand the intricacies of flight scheduling and delays, and evaluate the performance metrics of airlines and airports. The ultimate goal is to provide strategic recommendations to enhance operational effectiveness, improve customer experiences in air travel, and contribute to the overall advancement of the aviation industry's standards and practices.

#### Flights Dataset
This dataset contains detailed flight information, including timings, delays, and other flight-specific data.

#### Airlines Dataset
This dataset provides information about various airlines.

#### Airports Dataset
This dataset contains information about various airports.

## Excel Data Analysis: Manipulation, Formulas and Functions
#### 1. address missing data in the movies dataset. Are there any patterns in the missing data that can be noted
- Cancellations cause most missing values (departure, arrival, air time, etc.) → Filter using CANCELLED = 1.
- Diverted flights also lead to missing time fields → Use DIVERTED = 1 to isolate.
- Delay subcategories are missing only when delay didn’t happen → Fill missing with 0.
- Missing TAIL_NUMBER mostly tied to cancellations → Flag if needed.
- Latitude/Longitude missing for few airports → Filter out for mapping tasks.

#### 2. Determine the average flight delay per airline. What are the top 3 airlines with the highest average delays
Highest Delays
- American Airlines Inc. (23.19 min)
- Delta Air Lines Inc. (21.22 min)
- Atlantic Southeast Airlines (20.48 min)
Airlines like American Airlines and Delta show the highest average delays, while Frontier, Spirit, and Virgin America maintain more punctual performance. This data can help frequent travelers and analysts evaluate airline reliability based on past delay trends.

#### 3. Airport Traffic Volume
- Atlanta (ATL) is the busiest airport with nearly 8,800 flights, maintaining a narrow gap between outgoing and incoming flights.
- Chicago O’Hare (ORD) and Dallas/Fort Worth (DFW) follow closely, each with over 6,800 flights, indicating their major role as connecting hubs.
- Los Angeles (LAX) and Denver (DEN) round out the top five, reflecting high passenger and cargo traffic in the western U.S.
- These airports act as major national and international hubs, critical for both domestic connectivity and global transit.

#### 4. Flight Cancellation Insights
- American Eagle Airlines Inc. has the highest cancellation rate at 9.22%, significantly above the industry average. This suggests possible operational inefficiencies, resource constraints, or route/weather challenges.
- Regional carriers (e.g., American Eagle, Atlantic Southeast) tend to have higher cancellation rates, possibly due to more frequent short-haul flights and higher weather sensitivity.
- Major carriers like Delta, American, and United have moderate cancellation rates, showing relatively stable operations.
- Hawaiian Airlines shows exceptional performance with less than 0.5% cancellations — likely due to fewer routes and controlled weather environments.
- 
#### 5. Seasonal Variations in Flight Operations
- January shows a lower cancellation rate at 2.56%, despite having more flights, indicating relatively smoother operations.
- February has the highest cancellation rate at 4.14%, indicating increased disruption during this month. Possible reasons could include winter weather conditions, operational adjustments, or demand fluctuations.
- Overall Out of 70,000 total flights, 2,234 were cancelled, resulting in an overall cancellation rate of 3.19%.
- 
#### 6. Correlation between Distance and Delays
There is no strong correlation between flight distance and arrival delays. Short-distance flights show greater variability and more extreme delays, while long-distance flights tend to be more consistent with fewer significant delays. This suggests that factors other than distance—like airport congestion or scheduling—are more influential in causing delays.

#### 7. Efficiency of Airlines
Based on the percentage of flights that are not delayed, the top-performing airlines in terms of on-time performance are
- Frontier Airlines Inc. – 52.79% on-time rate (Rank 1)
- Hawaiian Airlines Inc. – 49.10%
- American Eagle Airlines Inc. – 48.41%
At the lower end, Delta Air Lines Inc. has the lowest on-time performance at 29.87%, despite being a major carrier.
Insight: The results show that regional and low-cost carriers like Frontier and Hawaiian are outperforming major airlines in maintaining on-time schedules. However, overall on-time rates are relatively low across the board, suggesting systemic delay issues in the industry.

#### 8. Impact of Day of Week on Flight Operations
Highest delays: Day 1 (Monday) — Avg. delay: 12.28 mins, Cancellations: 674
Lowest delays: Day 6 (Saturday) — Avg. delay: 3.24 mins
Lowest cancellations: Day 5 (Friday) — 146
Conclusion: Mondays see the most disruption; weekends (esp. Saturday) are smoother operationally.

#### 9. Analysis of Airport Connectivity
- Atlanta (ATL) is the most significant hub, serving 4,360 destinations, highlighting its central role in U.S. air travel.
- Dallas/Fort Worth (DFW) and Chicago O'Hare (ORD) follow closely, each serving over 3,400 destinations.
- Other key hubs include Los Angeles (LAX) and Denver (DEN), both connecting to over 2,500 destinations.
- These airports are critical nodes in the U.S. flight network, offering extensive connectivity and acting as major transfer points.

#### 10. Flight Duration Accuracy
-JetBlue Airways shows the highest deviation from scheduled times with an average ratio of 1.09, indicating longer actual flight durations.
- Hawaiian Airlines has the least deviation with a ratio of 0.97, suggesting it often completes flights slightly ahead of schedule.
- Most other airlines, including Delta, United, and Southwest, operate with a moderate deviation around 1.05–1.08, reflecting manageable scheduling variances.

#### 11. Airline Fleet Utilization
- Southwest Airlines has the highest fleet utilization, averaging 22.79 flights per aircraft, indicating high operational efficiency.
- American Eagle and SkyWest Airlines also show strong utilization with 22.28 and 20.27 flights per aircraft, respectively.
- Hawaiian Airlines and Atlantic Southeast Airlines maintain fleet productivity above 20 flights per aircraft.
- Higher utilization suggests better asset usage, while lower rates (e.g., United, Virgin America) may indicate underutilization or longer-haul focus.

#### 12. Airport Geographical Analysis
- The scatter plot visualizes the geographical spread of airports based on latitude and longitude.
- A high concentration of airports is evident in the central part of the plotted data.
- There are also sparser clusters of airports observed towards the bottom-left and bottom-right of the visualization.
- The scatter plot indicates the highest concentration of airports within the approximate latitude range of 25-50 and longitude range of -125 to -70, covering a large part of the contiguous US.
- TX State of US has the highest distritbution of airports which is 8724.

#### 13. Delayed Flights and Delay Types Analysis
- Analysis of delayed flights reveals that Late Aircraft Delay accounts for the largest proportion of the total delay time, with a sum of 321,528 minutes.
- This is followed by Airline Delay at 263,590 minutes.
- Weather Delay, totaling 45,967 minutes, contributes a smaller portion,
- and Security Delay represents the least amount of delay time at 1,090 minutes.
- Late aircraft issues and airline-related factors are the primary drivers of flight delays in this dataset.


#### 14. Long-Haul vs Short-Haul Operations
This comparison highlights that short-haul flights generally experience slightly higher average arrival delays than long-haul flights across most airlines. Airlines like JetBlue, American Eagle, and Skywest show notably higher cancellation rates for short-haul operations. The trend suggests that shorter routes may be more vulnerable to operational disruptions, possibly due to tighter scheduling and frequent takeoffs/landings.

## Dashboard
The dashboard provides a comprehensive overview of airline statistics, focusing on flights, delays, and cancellations. Here's a summarized insight

#### Overall Flight Operations:
- High Volume: The dashboard reports a total of 70,000 flights, indicating a significant amount of air traffic.
- Minimal Delays: The average departure delay is relatively low at 10.19 minutes, and the average arrival delay is even lower at 0.39 minutes, suggesting efficient operations overall.
- Low Cancellations: With 2,234 total cancellations out of 70,000 flights, the cancellation rate appears to be quite low, which is positive for passenger experience.

#### Flight Activity Trends
- Morning Peak: The "Number of Flights" chart clearly shows that the morning is the busiest period for flights (28,888 flights), followed by afternoon (21,871 flights). Evening and night see significantly fewer flights.

#### Airline Performance
- Key Metrics by Airline (Bar Chart - "Airline Key Metrics"): This chart likely breaks down average delays, total cancelled flights, and total flights for individual airlines (AA, AS, B6, etc.). Without specific values, it's hard to pinpoint top performers or underperformers, but it allows for quick comparison across airlines. Some airlines like VX and WN seem to have a higher number of total flights compared to others.
- Airline Delay Breakdown: This stacked bar chart details various types of delays (airline delay, air system delay, security delay, weather delay, late aircraft delay) for different airlines. This is crucial for identifying the primary causes of delays for each airline. For example, Southwest Airlines Co. and Skywest Airlines Inc. appear to have significant delays, with late aircraft delay and air system delay contributing noticeably. American Airlines Inc. also shows substantial delays.

#### Airport Activity:
- Top 10 Busiest Airports by Total Traffic: The pie chart highlights the airports with the highest traffic. ATL (Atlanta) is the busiest, followed by DFW (Dallas/Fort Worth) and ORD (Chicago O'Hare), which aligns with common knowledge of major US airline hubs. Other busy airports include LAX, IAH, PHX, DEN, MCO, and LAS

#### conclusion  
the dashboard paints a picture of a largely efficient airline industry with relatively minor delays and cancellations. While morning is the peak time for flights, specific airlines and airports stand out in terms of traffic and delay patterns. The detailed breakdown of delay types by airline is particularly useful for identifying areas for operational improvement








