# World Happiness

The World Happiness presentation is an interactive narrative visualization implemented as an interactive web page, using D3 programming in JavaScript. This was part of the Narrative Visualization Project for CS416 - Data Visualization at the University of Illinois Urbana-Champaign.

Link to running webpage: https://doananthony.github.io

# Summary

This narrative explores regional variations in happiness scores, correlations between happiness and healthy life expectancy, and emphasizes the multidimensional nature of happiness from provided worldwide data in 2018 and 2019.

# Write-Up

## Messaging

The message of the narrative is to explore and understand how different countries and regions from around the world score in terms of happiness scores. The nature of happiness is multidimensional, with different factors that impact it, such as GDP per capita, social support, freedom to make life choices, generosity, and perceptions of corruption. The narrative explores the correlation between these factors and also provides details on how happiness impacts a country’s healthy life expectancy. In summary, this website aims to provide insights and allow users better understanding of the complexity of happiness of different countries around the world.

## Narrative Structure

The structure that this narrative visualization was designed to follow is an interactive slideshow that included 5 total scenes (including a introduction and conclusion scene). Each of the main scenes focus on a specific aspect of the data with bar charts and scatter plots, with tooltips within all the charts allowing the users to navigate and explore the information in the bars or data points to get a deeper understanding of the factors that impact a country’s happiness. 

## Visual Structure

Each of the main scenes in the narrative visualization has a centralized visual structure that aids in the understanding of the data and navigating the scene. There is also a filter that allows users to select the year (2018-2019 since it was the data provided) to see how a year has impacted the scores of the various countries. 


- Scene 1 - Top 10 Happiest Countries: Contained a bar chart ranking the top 10 happiest countries in descending order with the scores being displayed on the x-axis. 
- Scene 2 - Happy vs Healthy: Displaying a scatter plot measuring the Healthy Life Expectancy on the x-axis and Happiness Score on the y-axis.
- Scene 3 - Regional Happiness: Grouping average scores of happiness of countries within a region and plotting it as a bar graph of all the regions and their average happiness scores in descending order.

The visual elements were used to highlight the important data points and guide the viewer’s attention to the key insights. Also, there were annotations on the charts as well as presented text to allow users to dive deeper into the data to get better insights. 

Finally, at the bottom of each scene were buttons to help users transition to the next scene (Continue button), with text before to help connect and transition into the next scene.


## Scenes

The narrative visualization had the following sequence of scenes:
- Introduction Slide: Introduce the presentation to the user
- Top 10 Happiest Countries: High level overview of the top happiest countries in the world
- Happy vs Healthy: Understanding the countries’ correlation between being happy and living a healthy life
Regional Happiness: Grouping average scores of happiness of countries within a region
- Conclusion: Wrapping up the presentation 

The scenes were put in this order because it helped tell the story about the data that was used for World Happiness. It begins with a brief introduction that provides the users an overview of the complexity of world happiness and what contributes to it. 

Then, the users go into the bulk of the presentation slowly with a brief overview bar chart of the happiest countries in the world with the ability to understand some of the factors that helped these countries score the highest. This would then let users wonder, “Why is this important?” which transitions into the next slide of Happy vs Healthy where we explore the scatter plot to show users the positive correlation between a happy and a healthy life. This scatterplot shows the group regions by color which leads us into the Regional Happiness scene where users get an understanding of the regions that averaged the highest scores in happiness as well as the factors that influenced it. Finally, the presentation wraps up with a conclusion. 

The structure of the scenes allow for users to become immersed in an interactive story that guides them through from beginning to end.


## Annotations

The template that was followed for all the annotations were tooltips that appeared when hovering over data points. This was chosen as it helped keep the visuals simple on the slide, while still providing more information, on-demand. Depending on the scene, the tooltip would provide more in-depth insights to help guide the viewers’ understanding of the data. The annotations served as textual cues that helped highlight different aspects that impacted the world happiness score, which helps emphasize how a country or region could score the highest or lowest in happiness score. These annotations were used to enhance the narrative and facilitate comprehension of the data and the presented scene.


The annotation changed based on the scene to help focus attention to the data that is being presented in the current visual. For example, the scatter plot’s tooltip would present metadata on a country’s happiness score, whereas the bar chart on the Regional Happiness scene has a tooltip that shows specific data for the average scores of the metadata of all the countries within that region. This shows that the annotations are able to be updated to adapt to the scene and helps users dive deeper into the data presented in the visual.

## Parameters

The first parameter of the narrative visualization would be the year that was used to help transition the visuals presented in the scenes. The data that was provided contained the happiness scores of all the countries in the world for 2018 and 2019. Within the narrative visualization, there was a year variable that was used to keep state of the current data that was displayed in the charts. The states of this would either represent the data for the year 2018 or 2019 of the presented charts. 


Another parameter used was for the window (window.location.href) to define the scenes and HTML files that go along with it. This is used to help keep state of the scene on where the viewer is within the narrative and to help transition between scenes with the help of triggers. These parameters are used to help define the state of the visualization and influence the content and presentation of each scene.

## Triggers

There were a few triggers used to help connect the actions to changes of state in the narrative visualization. There was the yearFilter variable that was used to store the current year displayed.  Within this, there was a defined method for on change that helped set the currentYear variable and update the plot to show the updated state in the visualization. The text that is provided in the scenes helped communicate that users are able to select the year. When the year filter is selected, it provides the options of the available years to select.

The next trigger that is used is for transitioning between scenes. Within the scripts, there were functions defined to transition the users between scenes in the slideshow, which provided the HTML file that the window would reference. These functions were placed on the onClick method within the buttons to trigger these functions when it was selected by the users. The buttons were provided at the bottom of each scene with provided text to communicate with the users on how they are able to navigate between the slides in the narrative. 
