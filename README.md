# Investment-ANALYSIS-KPI
🧩 Problem Statement

The management team of Capital Investment Group wants to evaluate the performance of different investment types, branches, and fund managers across Nigeria. They need to identify which regions and managers drive the highest returns, understand the risk exposure of the portfolio, and measure how effectively funds are performing over time.

🎯 Objectives

Evaluate investment performance across regions, branches, and fund managers.

Identify which investment types provide the best ROI and total return.

Understand how risk level impacts portfolio profitability.

Assess branch and fund manager contributions to overall investment value.

Provide actionable insights for strategic decision-making and investor engagement.

📊 KPIs (to calculate using DAX in Power Pivot)
KPI Name	Description	Example DAX Formula
1. Total Investment Amount	Total amount invested across all investors.	Total Investment = SUM(Investment[AmountInvested])
2. Average ROI (%)	Measures the average return on investment percentage across all transactions.	Average ROI = AVERAGE(Investment[ROI(%)])
3. Total Return Value	Total monetary value of returns from all investments.	Total Return = SUMX(Investment, Investment[AmountInvested] * Investment[ROI(%)] / 100)
4. Number of Active Investments	Counts how many investments are still active (based on maturity date > TODAY).	Active Investments = COUNTROWS(FILTER(Investment, Investment[MaturityDate] > TODAY()))
5. Average Duration (Months)	Calculates the average investment duration in months.	Avg Duration = AVERAGE(Investment[Duration_Months])
   
💡 2 Insights to Discuss

Regional Performance:
Lagos has the highest total investment value, suggesting stronger investor confidence in that region.

Top Performing Investment Type:
Bond investments, despite being low-risk, deliver stable returns over longer durations compared to crypto or real estate.
