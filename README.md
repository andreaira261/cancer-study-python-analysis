# Cancer Study Analysis 

## Overview 
In this assignment, an analysis of an animal study on squamous cell carcinoma (SCC) treatment was conducted to compare the performance of the drug of interest, Capomulin, against other treatment regimens. The data was cleaned and merged, and a summary statistics DataFrame, charts, and plots were generated using Pandas and Matplotlib. The findings offer valuable insights into potential anti-cancer treatments.

## Languages/ Tools: 
- Python
- Pandas
- Matplotlib

## Prepare the Data 
In this section, the dataset is prepared by merging the datasets into a single DataFrame and creating a cleaned DataFrame by dropping duplicate mouse records.
![data-prep-1](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/3d3b4a7d-ce87-45ce-b413-4952123f1822)
![data-prep-2](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/2edbad6f-8289-4d44-83e9-a30fd3a1cfd8)

## Generate Summary Statistics 
The mean, median, variance, standard deviation, and standard error of the mean of the tumor volume is calculated.
![summary-stats](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/212c0387-38f6-40ed-aef2-6725a47f17b5)

## Create Bar Charts and Pie Charts 
A bar plot displaying the total number of timepoints for all mice tested in each drug regimen is generated using Pandas and pyplot.
![bar-chart](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/b1faa802-033b-46ac-848a-c56a43fd9c0a)

A pie plot depicting the distribution of female versus male mice is generated using Pandas and pyplot.
![pie-chart](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/7585c595-66d0-4f55-bb55-691b83b7e289)


## Calculate Quartiles, Find Outliers, and Create a Box Plot 
A DataFrame, grouping mouse IDs and capturing their last timepoints, is created. The maximum timepoints are retrieved, and four treatment groups (Capomulin, Ramicane, Infubinol, and Ceftamin) are listed. 
![quartiles-outliers](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/a1ba4d32-899d-4952-8618-5fedb106311e)

A box plot is generated to depict the distribution of final tumor volumes for all mice in each treatment group, accompanied by interquartile range (IQR) and outlier details.
![box-plot](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/9863189a-a1bb-4d4b-a190-7afcf4b74be1)


## Create a Line Plot and a Scatter Plot 
A line plot illustrating tumor volume versus time point for a single mouse treated with Capomulin is generated. 
![line-plot](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/fe5f5d1c-748f-4e4e-9634-fb6a89b9f33e)

Additionally, a scatter plot depicting the relationship between average tumor volume and mouse weight for the Capomulin regimen is created.
![scatter-plot](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/e2578e53-99e0-44c1-9b21-e0b1c6684014)


## Calculate Correlation and Regression 
The correlation coefficient and linear regression model are calculated for mouse weight and average tumor volume for the Capomulin regimen.
![correlation-regression](https://github.com/andreaira261/cancer-study-analysis/assets/48165713/16b6b9e3-a3ea-4c56-b978-74d7693513b5)

## Analysis 
Based on the data from the animal study, several observations can be made to examine the performance of Capomulin against other treatment regimens. 

The bar chart displaying the total number of observed mouse timepoints for each drug regimen shows that Capomulin had the highest number of observations with 230, closely followed by Ramicane with 228 observations.

Moreover, when analyzing the tumor volume at the last observed timepoint for each mouse across the four regimens examined (Capomulin, Ramicane, Infubinol, Ceftamin), Capomulin showed the smallest IQR, indicating the least variability in the final tumor volume measurement. Ramicane also exhibited similar quartiles to Capomulin. In contrast, mice treated with Infubinol and Ceftamin displayed much larger quartiles in the final tumor volume, suggesting poorer efficacy in treating SCC compared to Capomulin and Ramicane.

Additionally, the line plot of tumor volume versus time point for Mouse l509 treated with Capomulin demonstrated that Capomulin was effective in reducing the tumor size after 45 days, with the most significant effect observed between days 20 and 35, as the tumor volume generally decreased during this period.

Lastly, a strong positive correlation of 0.84 was observed between mouse weight and average tumor volume for the entire Capomulin regimen, indicating a positive relationship between mouse weight and average tumor volume.

Overall, the study revealed that Capomulin and Ramicane generally had the best results compared to the other drug regimens tested.

