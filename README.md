# 2016-US-Presidential-Election-analysis
Introduction This report contains the presentation and analysis on the 2016 Election Results. Part A contains a Presentation 
on the election results for all states, including which States were won by Republicans and which states were won by democrats. 
In this section we highlight the results of the patterns characterized in this years election. To do so we eliminate the focus of 
geographic space and imply the focus of voting results by eliminating the eyes draw to a natural USA map. In doing so we hope to 
look towards the voting results and not just the geography.  Part B, attempts to present a county-wise result for the election.
It also attempts to establish a relationship between the average percapita Income of a Region and the Propensity to vote for 
the republican candidate.The results from two states are analyzed in detail: Michigan and Pennsylvaina. These states were chosen 
because the Presidential race was quite close in both these states. A regression analysis of the vote share for Trump vs county 
Percapita income is conducted for counties in each of these states. Programming Methodology Followed Part A uses the 'Chorogrid' 
function to loop draw shape geometries for the states. It then loops through these various states and plots the results on a colormap. 
1) The shapes are pre determined using the 'Chorogrid' module. They are essentially a blank slate that can be filled with data.  
2) In doing so we can choose to manipulate the shapes on a whim by both sections using manually gathered election data from the 
ap poll website and the new york times website.  3) We chose to focus this attention by using the module as such: 
to change the way the output of the maps is determined.  4) So we then assign the data to the various shapes and output the maps.  
In Part B the following procedure is adopted:  1) County shape files are imported and read using the Cartopy shp reader. 
These geometries are plotted on the USA map using the add geometries command in cartopy  2) For assigning republican and 
democratic counties a for loop is used on the shapefile.attributes dictionary. The county geometries are assigned inside the l
oop and assigned the facecolor 'red ' for republican and 'blue' for democrat  3) Results are analyzed in detail for the state 
of Michigan. to plot the various counties of Michigan, a for loop is used on the shapefile.attributes dictionary.
If the county is in Michigan, it is plotted. If it is republican , then it is plotted red, else it is plotted blue. 
The same procedure is adopted for plotting the ' Republican Voteshare' and the 'Per Capita Income' for the county 4) 
The same Procedure as in 3) is followed for the state of Pennsylvania  5) The seabon packeage and matplotlib packages are
used to pot the regression of ' Trump Voteshare' 'Per Capita Income'. The data points are plotted ' red' and 'bllue' using 
matplotlib and the regression line and confidence interval is plotted using Seaborn
