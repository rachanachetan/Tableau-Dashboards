# Enchantments permit lottery prediction 2024

### Synopsis: 
The team was tasked to provide analytics consulting services for an adventure outfitting company in Seattle called Northwest Treks, who seeked to secure a 4 day backpacking permit into the Enchantments in 2022 to create a promotional video with their team in the pristine alpine lakes region. Based on historical data, this interactive story board gives NWT reccommendations on which zone, day and group size to choose in order to win the lottery!

### The Challenge

Northwest Treks needs to fill out one application that includes three options: a first preference, a second preference, and a third preference.
Each preference allows them to specify the following choices:
- The preferred entry date
- The area of the Enchantments to visit
- The number of people in the party

Our team had to provide reccomendations for the above mentioned criteria and to answer these questions stated below: 

**Question 1.** What are the overall chances of winning the lottery based on 2021 results?

**Question 2.** What should they keep in mind as they submit their application? Are there specific selections that they can make in order to increase their chances of having their application accepted?

**Question 3.** If they want to be in the Core Zone of the Enchantments on days when the average historical temperature is over 52°F and the amount of rain is less than 0.03” on average, what date would you recommend they pick in order to increase their chances of having their application accepted?


### List of tools used:
Tableau for Visualization & Excel for data cleaning


### Data cleaning:
The steps followed for data cleaning are as follows: 

Step 1: Combining 2020 and 2021 lottery statatistics info from https://www.fs.usda.gov/detail/okawen/passes-permits/recreation/?cid=fsbdev3_053607

Step 2: Grouping and renaming zone names to retain only 5 final zones: Colchuck Zone, Core Enchantments Zone, Eightmile Caroline Zone, Snow Zone, Stuart Zone

Step 3: Remove unwanted columns

Step 4: Combine weather data from 1981-2022 from Historical Weather Data (Lat: 47.4785, Lon: -120.8192): https://prism.oregonstate.edu/explorer/

The cleaned data is saved as two .xlsx files containing weather data from 1981-2022 [here](/enchantments_weather_1981-2022.xlsx) and info on lottery statistics for 2021 and 2022 [here](/enchantments_lottery_results_2021-2022.csv). These are used as the data source for the dashboards built on Tableau.

### About the Dataset

#### Lottery statistics data (For 2020 and 2021):

Here is an overview of the permit applications in 2021 and 2022

<p align="center">
  <img src="/Enchantments/Introduction.png">
</p>

Other important criteria captured by the dataset include:
First preference, Second preference, and Third preference for the choice of zones.
Each preference allows them to specify the following choices:
- The preferred entry date
- The area of the Enchantments to visit
- The number of people in the party

#### Weather

The weather in the enchantments region ranges from -14.1 F to 79 F and the maximum precipitation received is recorded to be 5.83". 

The relationship between the success rate and the weather was analyzed to draw the following conclusions about the best time to visit the enchantments as follows:

<p align="center">
  <img src="/Enchantments/weatherdashboard.png">
</p>

### Result 

#### Overall chances of winning the lottery based on past results and specific conditions to keep in mind are:

<p align="center">
  <img src="/Enchantments/OverallRecco.png">
</p>

#### What NWT should pick in order to increase their chances of having their application accepted for the specific conditions of 1. Choosing the Core Zone of the Enchantments, 2. Average historical temperature being over 52°F and 3. The amount of rain being less than 0.03” on average:

<p align="center">
  <img src="/Enchantments/ReccoforProblemStmt.png">
</p>

Attached above are the screenshots of the built storyboards. You can download the Tableau [workbook](https://github.com/rachanachetan/Tableau-Dashboards/blob/main/Enchantments/Enchantments%20Final%20Project_Team_0221_FINAL-1.twbx) or find it hosted on Tableau Public: https://public.tableau.com/app/profile/rachana.chetan/viz/EnchantmentsFinalProject_Team_0221_FINAL/STORY for more information.

**This interactive storyboard was built by me along with my project team for our Data Visualization and Storytelling course taught by Prof. Ben Jones for the MSBA program at the University of Washington.**



