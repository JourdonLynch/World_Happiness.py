# World_Happiness

# Introduction

While happiness is inherently subjective, the World Happiness Index offers a structured way to examine the measurable factors associated with well-being across nations. This report analyzes key indicators within the dataset to determine how different variables influence perceived happiness and to identify broader trends in the drivers of societal well-being.

# Data Validation and cleaning

 The Pandas, matplotlib.pyplot, and seaborn libraries were imported to conduct the cleaning and analysis.

The initial dataframe from 2019 consisted of 135 rows and 10 columns
• The country column contained the object data type and consisted of the names of 135 countries included in the study and had no null values. No changes were made.

• The **social_support** column contained the float64 data type and ranked countries based on their social support. 1 null value was found and filled with the mean column value instead of removing the row.

• The **freedom** column contained the float64 data type and ranked countries based on their freedom. 1 null value was found and filled with the mean column value instead of removing the row. 

• The **corruption** column contained the float64 data type and ranked countries based on their corruption. 8 null value was found and filled with the mean column value instead of removing the row. 

• The **generosity** column contained the float64 data type and ranked countries based on their gnerosity. 1 null value was found and filled with the mean column value instead of removing the row.

• The **gdp_per_cap** column contained the int64 data type and consisted of the gdp of 135 countries included in the study and had no null values. No changes were made.

• The **life_exp** column contained the float64 data type and consisted of the names of  the lif eexpectancy of 135 countries included in the study and had no null values. No changes were made.

• The **happiness** column contained the int64 data type and consisted of the happiness scores of the 135 countries included in the study and had no null values. No changes were made.

# Exploratory Analysis

Happiness scores were broken down into seven distinct groups representing different regions. Europe, Oceania, North America, South America, Asia, and Africa. While Russia resides in both Europe and Asia, for the purpose of this analysis, it was placed in the European group as the majority of its population resides there. Asia and Europe have the largest interquartile range at 55, while Oceania has the lowest interquartile range at 1.50. North America, South America, and Africa exhibited outliers representing Haiti, Venezuela, and South Sudan, respectively.

Figure 1

<img width="616" alt="Screenshot 2025-02-16 at 9 31 03 PM" src="https://github.com/user-attachments/assets/776dae40-ca88-486d-a5a9-2966c712747e" />

#

The top 10 happiest countries were Finland, Denmark, Norway, Iceland, the Netherlands, Switzerland, Sweden, New Zealand, Canada, and Austria, respectively. Eight of the happiest countries reside in Europe while the remaining two are from Oceania and North America. The happiest country in the world was Finland with a happiness score of 155.

Figure 2

<img width="618" alt="Screenshot 2025-02-16 at 9 35 45 PM" src="https://github.com/user-attachments/assets/6a927f36-f03e-4d3b-b771-930287a5c685" />

#

The bottom 10 happiest countries in the world were South Sudan, Central African Republic, Afghanistan, Tanzania, Rwanda, Yemen, Malawi, Syria, Botswana, and Haiti, respectively. Six of the 10 least happy countries reside in Africa, with three of the remaining four residing in Asia and one being in North America. The least happy country in the world was South Sudan with a happiness score of 0.

Figure 3

<img width="619" alt="Screenshot 2025-02-16 at 10 05 14 PM" src="https://github.com/user-attachments/assets/f3c94162-f5a9-4b51-bbff-365ea55289d9" />


# 

In addition to happiness, countries were ranked on six different metrics: social support, freedom, generosity, GDP per capita, life expectancy, and corruption. To measure the impact different metrics had on the happiness of a country, the Pearson correlation coefficient was calculated, and countries were plotted using a scatterplot including a linear regression line. The closer a country's rank was to 1, the greater the social support, freedom, generosity, and GDP per capita it had, while also indicating lower corruption. A green to red diverging color map was used to indicate rankings from 1 to 143.

Figure 4

<img width="692" alt="Screenshot 2025-02-16 at 10 50 48 PM" src="https://github.com/user-attachments/assets/30a7d4fc-3a78-4638-88f5-8aa7d134fdf3" />

#

# Findings

• Oceania had the highest happiness with a mean happiness score of 146.5, although this may have been skewed as the region contained the fewest countries by far. Europe, South America, and North America ranked second, third, and fourth, respectively, with happiness scores of 109.8, 108.4, and 107.3, respectively. Asia ranked fifth with a happiness score of 72.1, while Africa was the least happy region with a score of 32.8.

• Social support, life expectancy, and GDP per capita were the three most influential metrics of happiness with correlation coefficients of -0.82, 0.78, and 0.73, indicating significant correlations. This means that as social support decreased, so did happiness, and as life expectancy and GDP per capita rose, happiness tended to follow.

• It was noted that corruption had a very weak negative correlation of -0.22, indicating that countries with high corruption aren't necessarily unhappy. In addition to this, freedom had a correlation of -0.57, indicating only a moderate effect. It was hypothesized that the impact of these metrics would be greater.

• Generosity presented a moderate negative correlation of -0.5, indicating that as generosity decreased, so did happiness. This was in line with expectations.

# Conclusion

Happiness varies considerably both within and across regions of the world. Although countries differ in cultural values and social structures, several common patterns emerge. Nations with higher levels of social support, longer life expectancy, and greater GDP per capita consistently report higher happiness scores. These factors are closely interconnected, as greater economic resources often support stronger social systems and improved health outcomes. While the idea that money cannot buy happiness remains widely accepted, findings from the World Happiness Report suggest that economic prosperity can significantly enhance the conditions that make higher levels of well-being more attainable.





