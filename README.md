<h2>1. Business Problem</h2>
Oil Extract is a fictional oil & gas extracting company. 
The Sector Manager sent an Excel worksheet containing information from the oil & gas area. He would like to understand the strategy for oil production 
considering the situations of "producing" and "injecting" wells, knowing that there is a relationship between them.
Then he asked to develop a reporting dashboard using the Microsoft Power BI and Python tools that generates insights for managerial levels, 
based on location, time, and other features about oil and gas wells, basins, and fields on land and sea.

<h2>2. Business Assumptions</h2>
The entire dataset, situation and solutions are completely fictionals and should not be related to any real situation.

<h2>3. Solution Strategy</h2>
<h4>3.1 Load data from XLSX worksheet;</h4>
<h4>3.2 Data treatment and cleaning on Python/Pandas;</h4>
Treating data in Python is considerably better than treating it in the Power BI Power M interface, 
as Python allows for better performance/speed and scalability during data processing.

- Assertive decisions and data treatment:
<h5>	* Rename and standardize column names, adopting abbreviations according to the data type (DS, NR, SG, etc.);</h5>
<h5>	* Standardize the first character to uppercase, allowing text standardization;                              </h5>
<h5>	* The COMPLETION DATE column was changed from datetime to date format;                                      </h5>
<h5>	* Rows with null data were deleted, as I found the guidance for treating this data confuse.                 </h5>

<h4>3.3 Export refined that to .parquet file;</h4>
It was chosen to generate a .parquet file instead of a .CSV file due to the significant gain in speed and storage size compared to CSV. 
Using the .parquet extension allows for more efficient work with large datasets.

<h4>3.4 Load .parquet file into Power BI and create Visual Dashboard with requested features:</h4>
<h4>- Apresentation/Visualization;</h4>
<h4>- Navigation through pages;   </h4>
<h4>- Filters cleaning;           </h4>
<h4>- Filters by:                 </h4>
<h4>  	* Field                     </h4>
<h4>  	* Basin                     </h4>
<h4>  	* Category                  </h4>
<h4>  	* State                     </h4>
<h4>  	* Completion Date (Between) </h4>

<h4>3.5 Create calendar dimension on Power BI:</h4>
A calendar dimension was created to be used as a reference in Power BI. This practice allows for performance gains in the utilization of time series data.

<h4>3.6 Exploratory data analysis using Python;</h4>

<h4>3.7 Analyze results and draw conclusions</h4>

<h2>4. Business Questions</h2>

<h4>4.1 Which states has more conclusions?</h4>
The top 5 states in number of conclusions are, respectively: Rio Grande do Norte, Bahia, Sergipe, Rio de Janeiro, Espírito Santo.

<h4>4.2 What is the worst state in number of conclusions?</h4>
The worst state in number of conclusions is Santa Catarina, located in South Region of Brazil.

<h4>4.3 What is the number of producting conclusions wells on the first state in number of conclusions and what this value represents related to the total number of conclusions?</h4>
The number of producting conclusions is higher on Rio Grande do Norte (3.305) and it represents 13% of the grand total number of conclusions.

<h2>5. Business Insights</h2>

<h4>5.1 The most productive region is the Northeast, accounting for 79% of oil and gas well production.</h4>

<h4>5.2 The 1980s to the 1990s were the most productive decades for oil and gas extraction.</h4>

<h2>6. Conclusion</h2>
The Power BI's Dashboard provides the possibility to analyse and get valuable insights into this specific data about oil and gas well performance, locations and well statuses, as well as a deeper look into some features and data values. For further or advanced analyses it could be necessary an assertive contact with the client.

<img align="center" src="https://github.com/cliffpk3/oil_extract/blob/main/img/dashboard.png"><img>

Also, part of the Power BI Dashboard visuals were recreated using Python, mainly Pandas, Matplotlib and Seaborn libraries and the result can be seen bellow.

<img align="center" src="https://github.com/cliffpk3/oil_extract/blob/main/img/python_charts.png"><img>


