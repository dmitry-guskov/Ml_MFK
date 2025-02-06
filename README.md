# **Flight Delay Analysis**  
This repository contains a solution to a short course on pandas exam (in russian)-- an exploratory analysis of flight delays using a dataset with 336,776 flights and 13 features. 
The analysis is performed in Jupyter Notebook (in russian)

### Dataset Description  

The dataset is presented as a **CSV file** containing **336,776 rows** and **13 columns**, including:  

- **year, month, day**: date of departure;  
- **dep_time, arr_time**: actual departure and arrival times (format **HHMM** or **HMM**), local timezone;  
- **dep_delay, arr_delay**: departure and arrival delays, in minutes. Negative values indicate early departures/arrivals;  
- **carrier**: two-letter carrier abbreviation;  
- **flight**: flight number;  
- **tailnum**: plane tail number;  
- **origin, dest**: origin and destination airports;  
- **air_time**: amount of time spent in the air, in minutes;  
- **distance**: distance between origin and destination airports.  

#### (For reference) New York airport abbreviations:  
- **JFK** — John F. Kennedy International Airport;  
- **LGA** — LaGuardia Airport;  
- **EWR** — Newark International Airport.  

---  

### Research Tasks  

1. **Which columns contain missing values?** How many rows have at least one missing value? Are there any specific patterns among flights with missing values? Remove all rows with at least one missing value from further analysis.  

2. **Plot normalized histograms** of **departure delay** and **arrival delay** on the same axes. Limit the histogram range to remove outliers and describe their characteristics (**count and values**). Are there any other notable features in the resulting distributions?  

3. **Calculate the mean, median, and standard deviation** for both **departure delay** and **arrival delay**.  

4. **Sort airlines by average departure delay** and provide the mean departure delay along with a **95% confidence interval** for each airline. Present the results as a graph.  

5. **Is the difference in mean departure delay significant** between **American Airlines (AA)** and **Delta Airlines (DL)?** At what significance level can we reject the hypothesis of equal means?  

6. **Compare departure airports (JFK, LGA, EWR) in terms of departure delays.** Are the differences statistically significant?  

7. **What type of distribution best describes departure delays** where **dep_delay > 0**? Suggest a general form of the distribution and estimate its parameters. Plot both a histogram and the probability density function of the fitted distribution.  

8. For flights where **dep_delay > 0**, **plot two graphs on the same axes**:  
   - The **number of delayed flights per month**;  
   - The **average departure delay per month**.  
   Compute the **correlation coefficient** between these values. Create a **scatter plot** showing their relationship (**X-axis: number of delayed flights per month**). Add a **regression line** and write down the **regression equation**.  

9. **Plot the average departure delay by hour of departure.** On a separate graph, plot the **proportion of flights with dep_delay > 0** by hour of departure. Provide a written description of the observed patterns.  

10. **Propose a method to classify airlines as punctual or non-punctual.** Which airlines belong to each group? Does punctuality depend on flight distance?  

11. **Develop a model to predict the average departure delay for each airport on the next day.**  
    - Which features will you use?  
    - What data will you use for training and testing?  
    - Evaluate the model's accuracy.  
    - Specifically, make a **prediction for December 31, 2013**, and compare it to the actual value (**excluding this date from training/testing**).  

12. **Find at least one additional interesting insight from the dataset** that reveals or characterizes patterns in the occurrence/distribution of flight delays.



License
This project is licensed under the MIT License.
