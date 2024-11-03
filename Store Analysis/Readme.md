# Sales Analysis Of Store
# Link -- https://app.powerbi.com/view?r=eyJrIjoiMGI2NjhlMGQtNDVkMS00YTlkLWEwOGUtZjM0MDhhZjFhOTM5IiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=a1a1290e25810b11ea97
# Description: 
The dashboard presents a comprehensive P&L and sales performance analysis across different segments, products, and countries. 
It includes:
Year-over-year performance comparisons
Segment and product profitability analysis
Geographical sales distribution
Discount analysis by segment
Sales trends and order metrics
Key performance indicators with goals.

# Key Learnings : 

# Financial Performance :

	1. Net Sales: 	118.73M (349.46% YoY growth)
	2. Profits: 	14.23M (-3.09% YoY decline)
	3. Gross Sales: 127.93M (347.93% YoY growth)
	4. COGS: 		101.83M (351.85% YoY increase)
# Segment Performance:
	1. Channel Partners: Highest profitability (72.4-73.7%)
	2. Enterprise: 		 Negative profitability (-1.2% to -7.0%)
	3. Government: 		 Moderate profitability (20.3-23.0%)
	4. Midmarket: 		 Strong profitability (25.6-28.9%)
	5. Small Business: 	 Low profitability (6.7-11.1%)
	
# Geographical Distribution:
	1. Top 5 Markets: 			USA, Canada, France, Mexico, Germany
	2. Highest orders: 			Canada (0.25M)
	3. ost consistent market: 	United States
	
# Discount Strategy:
	1. Varying discount bands (None, Low, Medium, High)
	2. Enterprise segment receives highest discounts (5.13-10.24%)
	3. Channel Partners maintains high profitability despite discounts
	
# Top 10 Questions for Analysis: 
1. Why is Enterprise segment showing negative profitability despite significant sales?
2. What factors contributed to the 349.46% YoY growth in Net Sales?
3. How can the profit decline of -3.09% be addressed while sales are growing?
4. What best practices from Channel Partners can be applied to other segments?
5. Is the current discount strategy optimal across segments?
6. Why does the Small Business segment show low profitability despite moderate discounts?
7. What drives the success in the Canadian market for total orders?
8. How can Enterprise segment profitability be improved without affecting sales volume?
9. What causes the variation in manufacturing costs across products?
10. Are there opportunities to optimize COGS given the 351.85% YoY increase?

# Important DAX Formulas: 
	1. Year over Year Change:
		YoY Change = 
		CALCULATE([Current Value]) - CALCULATE([Prior Year Value])
		
	2. Profit Percentage:
		Profit % = 
		DIVIDE([Profits], [Net Sales], 0) * 100
		
	3. YoY Growth Percentage:
		YoY Growth % = 
		DIVIDE(
			[YoY Change],
		CALCULATE([Prior Year Value]),
		0
		) * 100
		
	4. Segment Profitability:
		Segment Profit % = 
		CALCULATE(
			AVERAGE([Profit %]),
			GROUPBY(Sales[Segment])
		)
	5.Discount Impact:
		Discount Impact = 
		DIVIDE(
		[Total Discount Amount],
		[Gross Sales],
		0
		) * 100
		
# Report Summary
The dashboard reveals a complex business performance picture:

	##Strengths:

		1. Exceptional YoY growth in sales (349.46%)
		2. Strong Channel Partners segment performance (>72% profit)
		3. Robust geographical diversity
		4. Effective performance in key markets
	##Challenges:

		1. Declining overall profits (-3.09%)
		2. Negative Enterprise segment profitability
		3. Variable discount effectiveness
		4. Rising COGS (351.85% increase)
	## Opportunities:

		1. Enterprise segment profitability optimization
		2. Discount strategy refinement
		3. COGS management improvement
		4. Small Business segment enhancement
		5. Geographic expansion based on successful markets
		
The dashboard effectively tracks crucial business metrics and highlights areas requiring strategic intervention, 
particularly in profitability management and cost control despite strong sales growth.

# Snapshot -- 


