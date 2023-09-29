# LHL-Midterm-Project

## Project Goals

There are too many car accidents and far too many lives lost from them.  We believe that advertising the same message to an entire population is not the most effective method for capturing their attention and conveying the critical information that they need know.  We feel that developing an age-specific approach in advertising is a more impactful strategy.  In order to achieve this, we will conduct a thorough analysis of the collision data to find specific insights and information, which will further the ability to engage and captivate our target demographics.

Our Stakeholders in this project are the State Officials who would create the advertising campaigns to reduce collisions.  We seek to prove to them why we should take a more age-driven advertising approach and then create a user friendly, intuitive, and effective dashbaord that can be used to collect these age-driven insights.

## Process

1.  Take an exorbitant amount of time searching the world for an interesting dataset.

2.  Extract collision data from DB using SQLite.
    - See File: "DB_Extraction.ipynb"

3.  Using Python to conduct a thorough cleaning process and comprehensive exploratory data analysis to become familiar with the data and how it can be leveraged to acheive our goals.
    - See File: "Collisions_Cleaning_Engineering.ipynb" --> Cleaning, modification, and engineering of tables.  
    - See File: "EDA_Statistics_ProbabilityCalculations.ipynb" --> Exploration, Analaysis, Insights used to justify the project goals.

4. Structuring of the data into meaningful arrangements and creating interesting and informative visualizations in order to better convey the importance of the message and give insights on how to reduce the number of collisions by appropriately engaging the specific age groups.  

# Results

Our first objective was to provide enough evidence to justify and convince State Officials that age-specific advertising and collision awareness would be a more effective strategy than simply advertising in broad strokes accross the entire population.  In order to show this, we needed to prove that there is substantial enough variation in collision data between the distinct age groups.

When comparing the ratio of fatalities to the ratio of collisions by the hour, we observed that there are times of the day that are far more dangerous than others.  Despite the fact that the busiest times of the day indeed translate to more collisions during those times, these were not the times with highest ratio of fatalities per collision.  It was actually the least busy driving times of the day that proved to have the highest ratio.

<img src="images/ratio_of_fatalities_to_collisions.png" alt="Proportion of Fatalities to Collisions by Hour" width="400" height="300">


Key Take-aways:
- An accident that occurs in the early hours of the morning (between 1 - 4am) is up to 4x more likely to be fatal than accidents that occur during peak traffic hours (between 3 - 6 pm).
- If the amount of cars on the road or even number of accidents per hour are not contributors to this observation, something else is causing this disproportionate rate in fatalites in the early morning collisions.

New Questions that emerge:
- Could it be the cause of the accident that drives this observation? Is there more speeding, driving under the influence, tired driving happening during this time?
- Could it be that people display different driving habits and practices during these times, such as not wearing a seatbelt, or using their phones.
- Is this observation age specific? Or is this proportionality consistent accross age groups?

While exploring this last question of whether this is age specific, we found that the general distributions of the ratios of fatalities to collisions was consistent across age ranges.  However, we saw a stark difference in the overall probability of fatalities between these groups.

<table>
  <tr>
    <td><img src="images/fatality_rate_by_hour10-29.png" alt="" width="300"></td>
    <td><img src="images/fatality_rate_by_hour30-49.png" alt="" width="300"></td>
    <td><img src="images/fatality_rate_by_hour50-69.png" alt="" width="300"></td>
    <td><img src="images/fatality_rate_by_hour70plus.png" alt="" width="300"></td>
  </tr>
</table>

Taking the average fatality rates for all hours for each of the different age groups to compare these rates to one another, we can see more clearly how the different groups face different risk of fatality.

<table>
  <tr>
    <td><img src="images/at_fault_age_distribution.png" alt="Age Distribution of At-Fault Parties" width="300">
    <td><img src="images/avg_rate_of_fatalities_by_age.png" alt="Average Fatality Rate By Age" width="300">
  </tr>
</table>

When comparing this chart to the distribution of collisions by age, we can see that as the age of the driver increases, the number of collisions decreases. This might cause us to believe that the most dangerous drivers on the roads are ages 15 - 30. However, when we look at the fatality rates, we see that the older someone gets, the more likely their collision will result in a fatality. Thus, fatality rates by age and the number of collisions by age are inversely proportional. In other words, even though there may be more accidents caused by younger drivers, we see that the nature of collisions grow increasingly more fatal as drivers get older.

Admittedly, there may be other factors at play here. It could be something as simple as the older you get, the more frail you get, and thus are more likely to be killed in an accident. Although, the underlying issues that cause this observation is likely more complicated than that.

After diving a little deeper into the specific causes of collisions, we found that some were definitively more prevalent amongst different age groups. For example, DUIs were more prevalent among those ages 20-40, whereas falling asleep behind the wheel more prevalent among the more aged population.

<table>
  <tr>
    <td><img src="images/dui_dist.png" alt="Age Distribution of DUIs" width="300">
    <td><img src="images/falling_asleep_dist.png" alt="Age Distribution of Falling Asleep Behind the Wheel" width="300">
  </tr>
</table>

Key-Insights:
- Ages 20-40 are 20% more likely to be driving under the influence than a person in their 40s, 50% more likely to be driving under the influence than a person in their 50s, and 100% more likely to be driving under the influence than a person in their 60s.
- The ratios are fairly even across the age-groups, but we do see a small uptick in drivers between the ages of 30-39, but a major increase (by nearly 3 times) in the 80-89 range.

We conclude that it's been made clear that there are certain causes of collisions that are more prevalant for one age group that is not as prevalent for the next.  Thus, when it comes to marketing and advertising campaigns aimed at the public to minimize accidents and associated injuries or fatalities, a one-size-all approach may not be the most effective method. We should instead be tailoring the advertisments to speak directly to the different age-groups in order to capture more people's attention, whereby being more effective in generating awareness of collisions and hopefully encourage better driving habits.

Next Steps:
We will use Tableau to create dashboards for our State officials to use and interact with to glean more specific collision details for each age-group.

## Challenges?

## Future Goals


