2.	Part 2(a) 
In this task, we are required to find such days of the week and time that will help us to minimize delays. 
First, we start with the best time. For that, it was decided to calculate a “proportion of delayed flights for each time range”. For that, we defined function “calculate_delay_proportion(df)”. Then, we counted “the total number of flights and the number of delayed flights (where arrival delay is greater than 0) for each group.” After that, we, “dividing the number of delayed flights by the total number of flights, have obtained the proportion of delayed flights for each group.” After that it was decided to use bar plots where the minimum bar will show the best time to minimize 
delays. 
![image](https://github.com/puper26/Flights-analysis/assets/47867006/37e36fb0-0d07-4189-9f63-f954c579da07)
3.	Part 2(b)

For this task, we are required to identify if older planes suffer more delays than new planes. 

It was decided to use a “test for difference in proportions at 5% significance level”. “The age of each plane is calculated by subtracting its manufacturing year from the current year”, while the proportion of delayed flights (defined as departure delay exceeding 15 minutes) is calculated separately for old (plane age >= 20 years) and new planes (plane age < 20 years). 

A two-sample t-test is conducted to compare the mean departure delays of old and new planes. This test assesses whether the difference in delays is statistically significant: 

Hypothesis 1: “Old planes do not suffer more delays than new planes.”

Hypothesis 2: “Old planes do suffer more delays than new planes.”

Output: 
Year: 1998
Proportion of delayed flights for old planes: 0.15661161256345363
Proportion of delayed flights for new planes: 0.15079584733985057
T-statistic: 4.649007714823757
P-value: 3.3515157024305223e-06
There is a significant difference in the proportion of delayed flights between old and new planes at 5% significance level

Year: 1999
Proportion of delayed flights for old planes: 0.12053544339130329
Proportion of delayed flights for new planes: 0.15612890933900433
T-statistic: 7.340953613249759
P-value: 2.193073654318063e-13
There is a significant difference in the proportion of delayed flights between old and new planes at 5% significance level
![image](https://github.com/puper26/Flights-analysis/assets/47867006/685d86d5-f9fa-491e-9a9e-73467d528e4f)

4.	Part 2(C) 

The analysis utilizes logistic regression to model flight diversion probability from 1998 to 2007, incorporating features such as month, day of the week, departure delay, and flight distance. Feature engineering enhances predictive capabilities by introducing binary indicators for late aircraft, weather delays, and carrier-related issues. Model performance is assessed through training-testing splits, and coefficients are visualized to discern feature influences. This iterative approach provides insights into evolving trends and patterns, aiding in the formulation of targeted strategies to mitigate flight diversion risks and enhance aviation safety.



 
![image](https://github.com/puper26/Flights-analysis/assets/47867006/cc9c8e8c-8720-4bff-94f5-84490eeae4b9)
