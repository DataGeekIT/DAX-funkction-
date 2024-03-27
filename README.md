# DAX-funkction- increase, decrease, or no change in the metric

**Calculation Name: Growth1**

Description: The Growth1 calculation in DAX (Data Analysis Expressions) is designed to evaluate the growth of a certain quantity metric over time, focusing on monthly intervals. It compares the current month's quantity with the quantity from the previous month to determine if there was an increase, decrease, or no change in the metric.

**Formula Explanation:**

The calculation begins by calculating the sum of the quantity metric for the current month using the DATESMTD function. This function aggregates data from the beginning of the current month up to the specified date.
It then calculates the sum of the quantity metric for the previous month using the DATESMTD function in combination with PREVIOUSMONTH, which aggregates data for the previous month.
Next, it evaluates whether the current month's quantity is greater than, equal to, or less than the previous month's quantity, and assigns a corresponding growth status code (1 for increase, 0 for no change, and -1 for decrease).
Finally, the calculation returns the growth status code for further analysis.
Usage: This calculation is useful for tracking the performance of a quantity metric over time, particularly on a monthly basis. It provides insight into whether the metric is trending upwards, stable, or declining, helping users to identify patterns and make informed decisions based on the data.
