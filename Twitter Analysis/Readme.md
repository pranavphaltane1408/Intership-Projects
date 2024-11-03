# Twitter Analysis

# Link--https://app.powerbi.com/view?r=eyJrIjoiZThmMDIwOTktMmE0Ny00NTUzLWE5M2YtMGYyNmM1NTBjOWRlIiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=81fc14f128d0a720608a

# Description: 
The dashboard presents a social media analysis focusing on Twitter performance metrics, including:
Tweet engagement metrics,
Temporal distribution of tweets,
Media engagement and views analysis,
Top performing tweets by URL,
Overall engagement rates and impressions,
Weekly posting patterns.

# Key Learnings:

# Engagement Metrics:
	1.Average Impression: 		595.08
	2.Average Engagement Rate: 	3%
	4.Total Tweet Count: 		223
	5.Average Media Engagement: 13
# Posting Patterns:
	1. Highest activity: Tuesday (67 tweets)
	2. Second highest: Monday (39 tweets)
	3. Lowest activity: Saturday (12 tweets)
	@ Clear weekday preference over weekends.
# Content Performance :
	1. Top performing tweet: 57 engagements
	2. Second highest: 		 31 engagements
	@ Steady decline in engagement from top to bottom performers.

# Top 10 tweets show significant engagement variance:
	1. Media Performance
	2. Correlation between media views and engagement
	3. Visual representation shows positive relationship
	4. Consistent engagement patterns across media content.
	
# Top 10 Questions for Analysis:
1. Why is there such a significant drop in posting frequency between Tuesday (67) and other weekdays?
2. What characteristics do the top performing tweets share that lead to higher engagement?
3. Is the 3% average engagement rate meeting industry standards for the relevant sector?
4. How does the media engagement correlate with overall tweet performance?
5. What factors contribute to the low weekend posting frequency?
6. Are the average impressions of 595.08 meeting target audience reach goals?
7. What types of media content generate the highest engagement?
8. Is the current posting schedule optimal for the target audience?
9. How do engagement patterns vary throughout different times of the day?
10. What strategies could improve the performance of lower-performing tweets?

# Important DAX Formulas:
	1. Average Engagement Rate:
		Avg Engagement Rate = 
		DIVIDE(
		SUM(Twitter[Engagements]),
		SUM(Twitter[Impressions]),
		0
		) * 100
		
	2. Daily Tweet Count:
		Tweets by Weekday = 
		CALCULATE(
			COUNT(Twitter[TweetID]),
			GROUPBY(Twitter[WeekDay])
		)
		
	3. Media Engagement Ratio:
		Media Engagement Ratio = 
		DIVIDE(
		[Total Media Engagements],
		[Total Media Views],
		0
		)
		
	4. Rolling Average Impressions:
		Rolling Avg Impressions = 
		CALCULATE(
			AVERAGE(Twitter[Impressions]),
			DATESINPERIOD(
				Twitter[Date],
			LASTDATE(Twitter[Date]),
			-7,
			DAY
			)
		)
		
	5. Engagement Performance Index:
		Engagement Performance = 
		DIVIDE(
			[Current Period Engagement],
			[Previous Period Engagement],
			0
		) * 100
		
# Report Summary : 
The Twitter analytics dashboard reveals several key insights and opportunities:

	## Strengths:

		1. Consistent weekday posting schedule
		2. Strong Tuesday engagement
		3. Clear tracking of media performance
		4. Detailed engagement metrics
		5. Areas for Optimization:

	## Weekend Content Strategy: 
	
		1. Currently underutilized
		2. Opportunity for audience growth
		3. Potential for different content types
		4. Engagement Distribution
		5. Wide variance between top and bottom performers
		6. Need for content strategy refinement
		7. Opportunity for engagement improvement
		8. Media Performance
		9. Strong correlation with engagement
		10. Potential for optimization
		11. Opportunity for content type diversification
		
	## Recommendations:

		1. Investigate successful Tuesday content strategy for application across other days
		2. Develop targeted weekend content strategy
		3. Analyze top-performing content characteristics for replication
		4. Optimize posting schedule based on engagement patterns
		5. Enhance media content strategy based on performance metrics

The dashboard effectively tracks social media performance and provides actionable insights for content strategy optimization and engagement improvement.

# SnapShots -- 
