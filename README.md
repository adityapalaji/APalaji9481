BrainStroming

Migration is part of human life. Migrations to and from a place determine the activity in the places. For example cities in Texas are growing fast but cities in mid west are suffering. Houston may overtake Chicago to be the 3rd largest city in US in next 5-10 years. We plan to capture migration at state level. We want to represent this in cloropleth-map which shows migrations at state level.

Data Source

We are using IRS migration data source and State level flows. The template and data sources are in this repository. We are taking migration stateinflows state outflows data from 2008 onwards

Cleaning and ModellingData

After we read the data from the data files we used pandas to create dataframes which combine all these files into two data frames one containing stateinflows and the other containing state outflows. We added a year column in these data frames to determine the returns in that year.

Data Representation

We used ipywidgets create a widget which takes input of from state and to state. We used matplotlib to display the graph (sample screen shot link)

Issues Faced

We tried to create a cloropleth-map which on hovering over state would siplay the migration of the state. The top states where outflow occurs from this state and top states from which inflow occurs to this state. Unfortunately we could not find an open source library to do this. Googles library did not have functionality to add on hover and other functions.Plotly have this feature but it is a paid service
