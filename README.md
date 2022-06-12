# Analysis Overview

I have been given the task of analyzing the data for the Citi Bike bicycle sharing service in New York City. Myself and a colleague are interested in implementing a similar bike sharing service in Iowa, but in order to do this successfully we need do a deep dive on the data provided to us in a CSV file which contains NYC's Citi Bike information. 
Using VSCODE and my skills with Python and Pandas, I first created a dataframe of the provided CSV file. I then converted the tripduration column to the Datetime format so that I could be more efficient at creating my charts in Tableau. I then exported this new dataframe with the converted column to a CSV file and headed over to Tableau to do the rest of my analysis.
In Tableau I began with loading my CSV file. I made various charts and created a Tableau story which I will share below. 

# Tableau Visualizations and Descriptions

![Checkout Times for Users](https://user-images.githubusercontent.com/100390727/173246715-21baee70-7e08-4bed-83b6-b393c5098619.png)

The first Visualization I created was a line chart that describes the checkout times for bikes by Citibike users. On the X axis is minutes of trip durations and on the Y axis is the number of registered bikes. I filtered this graph by the hours of trip duration, and have displayed hours 0-2. The peak of this line chart is at hour 0 and minute 5 with 146,752 bikes being used.

![Checkout Times by Gender](https://user-images.githubusercontent.com/100390727/173246895-468cab2f-f42b-43c8-bab1-ae3ae075302b.png)

The second visualization I created was another line chart similar to the one above. I filtered this data to show the checkout times by Gender. There are 3 genders recorded in our data: Female, Male and Unknown. We can see by this chart that males have the most checkout times, followed by females and then the unknown gender.

![Trips by Weekday per Hour](https://user-images.githubusercontent.com/100390727/173247012-4898bd29-b4a4-449a-b8ce-a23532217da1.png)

I then created this neat heatmap which displays the count of trips for each weekday and hour. On the X axis are the abbreviated days of the week and on the Y axis are the hours of each day. The darker the color of this map, the higher the number of rides that are being taken at that time. According to this visualization the bikes are being checked out the most between about 6am-9am and then again between 5pm-8pm on weekdays. Saturdays and Sundays seem to have a good amount of riders in the middle of the day. This data can certainly be useful to us when it comes to implementing our own service in Iowa.

![Trips by Gender (Weekday per Hour)](https://user-images.githubusercontent.com/100390727/173247229-dc04fd60-37f5-437e-bdba-f32ecfac1c4e.png)

Another heatmap was created, very similar to the one above, except I broke it down by our 3 different reported genders. We can see by this graph how popular the bikes are at different days amongst females, males, and unknown genders. It appears that the male heatmap has darker colors, which means that there are a large amount of males using the bikes throughout the day. The unknown gender heatmap is the lightest of the 3, meaning that there aren't a significant amount of riders claiming this gender on any given day.

![User Trips by Gender by Weekday](https://user-images.githubusercontent.com/100390727/173247356-443c812d-de14-4fab-a48a-e4645b6f113e.png)

This next visualization also analyzes user trips by Gender and by the days of the week. What I have included in this graph is the difference between customers and subscribers and how often each of these two categories are using this bike sharing service. We can see by this heatmap that the most popular demographic for these bikes are male subscribers. Subscribers in general are using these bikes much more frequently than regular customers. This is really helpful for us because we can see that having a subscription to bike sharing services is a great idea and will pay off.

![Bike Repairs](https://user-images.githubusercontent.com/100390727/173247672-b27910b4-33b0-430d-a702-0f07bd0cdad8.png)

This stunning treemap is a representation of bikes that may be due for repair. The darker colors are at the top left of the graph while the lighter colors are off to the right. Each of these tiny squares represent different bikes and how often they've been used. The bikes that have been used more frequently are most likely whethered and have issues of some sort that may need to be attended to. By creating this chart, one could locate these bikes by their ID numbers and inspect them to see if any repairs are neccessary. 

![Bike Utilization](https://user-images.githubusercontent.com/100390727/173247796-6a965b73-b43a-4ca5-a57d-6918014b4a30.png)
This last visualization is a large circle comprised of smaller circles which represent every bike in our data. Theh larger circles are on the outside of the chart while the center of the large circle is made of the smaller circles. In this case, the larger dots are the bikes that have been utilized more frequently. The dots that are smaller and toward the center are the bikes that have a smaller utilization rate. We could also use this graph to tell us which bikes need attending mechanically and which ones are most likely in good condition. By analyzing the location of the bikes with higher utilization we could make a pretty good conclusion on which locations in NYC are the most popular for these Citi Bikes.

# Summary

All in all, Tableau has proven to be a highly affective application when it comes to visualizing a data and telling a story. The graphs that I have produced are simple to understand and don't require any high-level data analysis experience to comprehend. The Citi Bike CSV file that was provided to us may seem intimidating if one were to glance at the file itself. Putting this file into a dataframe, with pandas for example, can make this data much more readable and easier on the eye. Tableau adds an even better representation of this data with the various types of visualizations we can create.
After completing this analysis, I feel much more confident about our plan to operate our own bike sharing service in the state of Iowa. We now know the length of most trip durations, the genders of the people who are renting these bikes, the most popular times of day that these bikes are being utilized, and much more. This information will help us immensely with our business plan. 

There are two visualizations that believe would also be beneficial in understanding bike sharing services:

1. The ages of riders. It would be great to look at how old the average Citi Bike rider is so that we could market to that demographic. We could see how many kids under 18 years old are using this service and we could also see how popular this service is with elderly folks.
2. Accidents. I'm curious as to whether or not these bike sharing services are dangerous. With customers especially (versus subscribers) it's very possible that perhaps someone is in the city as a tourist and doesn't quite know how to navigate around, which could be dangerous. I also suspect that there are a high level of intoxicated people who use this service. If we had data of how frequent accidents are with Citi Bikes, we could perhaps take certain cautions when it comes to creating our own business.

[link to dashboard]https://public.tableau.com/app/profile/adam.joy3740/viz/NYC_CITI_BIKES_16550544736460/CitiBikeStory

