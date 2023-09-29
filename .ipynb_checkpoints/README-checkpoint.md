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

!['Ratio of Fatalities to Collisions'](images/Ratio of Fatalities to Collisions.png)

Key Take-aways:
- An accident that occurs in the early hours of the morning (between 1 - 4am) is up to 4x more likely to be fatal than accidents that occur during peak traffic hours (between 3 - 6 pm).
- If the amount of cars on the road or even number of accidents per hour are not contributors to this observation, something else is causing this disproportionate rate in fatalites in the early morning collisions.

New Questions that emerge:
- Could it be the cause of the accident that drives this observation? Is there more speeding, driving under the influence, tired driving happening during this time?
- Could it be that people display different driving habits and practices during these times, such as not wearing a seatbelt, or using their phones.
- Is this observation age specific? Or is this proportionality consistent accross age groups?

## Challenges?

## Future Goals


