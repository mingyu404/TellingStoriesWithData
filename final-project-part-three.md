| [home page](https://mingyu404.github.io/TellingStoriesWithData/) | [visualizing debt](visualizing-government-debt) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# The final data story

Shorthand Link: [https://preview.shorthand.com/j9eDxYmtQYQrQwbH](https://preview.shorthand.com/j9eDxYmtQYQrQwbH)

# Changes made since Part II

I changed almost all of my visualizations from Part II. Here is the details and rationale:

- **Basic**

  + Aside from Tableau, I used Common Ninja and Flourish as visualization tools since I found them fit better with Shorthand in terms of size and interaction. I found although Tableau is good at dealing with large dataset and doing some initial sketches and EDA to observe the patterns and distributions of variables, these online tools, Common Ninja and Flourish, provides more options for visualization and are more flexible if and only if I can narrow down the range/size of data to show -- they are not convenient or not able to use an imported data. Therefore, when I used these online tools, I just manually entered the data that I wanted to show. However, the drawback is the free plan of Common Ninja cannot hide the ads, which is relatively evident (but acceptable I think)...
  + Changed the background color for all of my visualizations to better sync the theme color.
  + Deleted the news section based on feedback from Part II.
  + Changed the layout of the entire storyboard to be vertical in all sections for consistency.
  + Changed the color of highlighted numbers to better differentiate them from the headings, which I think is particularly useful in the *factors contributing to collisions section*.
  + Change since Part 1: I changed the original bubble chart visualization for *factors contributing to collision in New York* to word cloud. The reason is that the word cloud can clearly show the full and more words. I don't make it interactive and use a bar chart to show the exact numbers  because I think it is unnecessary and redundant -- I want people to notice the main factors contributing to collisions without distraction by numbers. In this case, I think different sizes based on exact numbers are already enough for intuitive understanding.

- **Visualizations of the number of collisions, people injured and killed from 2021 to 2022**

  + I used 3 line charts for these three elements for consistency. Also, the line chart can better illustrate the change/trend over time. It's not practical to put them all in one chart due to scale differences as mentioned in *Part II Identified changes for Part III*.

- **Map showing the collision frequency from 2012 to 2022**

  + I used a circle to highlight the critical change in data points over time in the map so that such change can be more evident to the audience, reflecting on the interview results.
  + Also, I changed the transitions to "Fade" to better show the gradual change over time. This can also make the transitions more obvious to readers.

  ![image-20231204023704282](/Users/zhangmingyu/Library/Application Support/typora-user-images/image-20231204023704282.png)

- **Bar charts of the most dangerous streets**

  + Only included the top five most dangerous streets, reflecting on the feedback in the critique group in the class.
  + Changed the background image to a map that highlights these 5 dangerous streets shown on the bar charts for better engagement (although I adjusted the color to be pretty dark for better focus).

- **Collision frequency by hour**

  + I found in my previous version I didn't filter the year when showing collisions by hour and just showed the total volume of collisions by hour over the past 10 years, which is actually problematic. Therefore, I re-selected the data, added the filter to include only the recent 3 years, and created 3 area plots for these 3 years in one chart to better show the consistency of the hourly collision patterns.
  + I change the labels for the horizontal axis from *"0, 1, 2, 3, ..., 23"* to *"12:00 AM, 1:00 AM, 2:00 AM, 3:00 AM,..., 11:00 PM"*, which I think is more intuitive for people.

- **Collision frequency by weekday & by season**

  + I dropped the unreadable bar charts and also used the area chart for these two visualizations since area plots, in this case, can better show the consistency and the general pattern and importantly, are more readable.
  + I also condensed the number of years displayed since I think it is unnecessary to include all years if their patterns are similar. Therefore, including just a few years can show the general pattern or specific anomaly. 

- **Main vehicle types**

  + I changed the original one to pictogram charts (bar charts with icons) so that readers will be able to compare the proportions of different types of vehicles involved in crashes more intuitively.

- **Injuries/fatalities by motorists, pedestrians, and cyclists**

  + Previously, I plotted three lines in one chart for these 3 groups of people, but I later found that the value in the Y-axis would be wrong and so would the position of lines if I plotted three lines in one chart in Tableau. Also, I found the initial visualization is not that intuitive and meaningful since people can only know motorists account for the greatest share of injuries and fatalities through the line charts, with no specific numbers or interesting findings, which seems to be common sense in this story setting...Therefore, I made the following modifications:
  + I calculated the average percentages for these three groups of people in terms of injuries and fatalities and found the proportions of injuries are quite consistent over the past 5 years, so I used a pictogram chart to show the average percentage of motorists, pedestrians, and cyclists directly. Hovering over the visualization lets the reader see the exact percentage figures directly. Also, different icons in this case, also help intuitive understanding. I did not separate these three groups of people into three individual bars here since my intention is not to compare the proportions but to show the average percentages for readers.
  + In terms of the *Average Proportion of Fatalities*, after calculating the percentage share, I found an essential fact that pedestrian deaths rose from 38% to 50%, while fatalities among motorists have seen a decrease from 52% to 43% from 2020 to 2022. I think it is quite important for people to learn about the change in proportional fatalities/vulnerability over the years. To visualize this newly found fact, I chose to use bar charts with icons to directly show the change between 2020 and 2022, which I think is more intuitive for people when learning this fact. I don't use the pie chart in this case since the absolute numeric changes are not that much -- even though a 12% proportional fatalities increase to pedestrians actually means a great difference -- so a pie chart cannot show such changes well and will make it hard for people to compare proportions in two different years. 

- **Conclusion/Call to Action**

  + I modified the conclusion part to be more targeted to my target audience by including specific suggestions for my target audience based on the hourly, weekly, and seasonal patterns and the top contributing factors to the vehicle collision analyzed earlier in the story, reflecting on the feedback of the interview.

- **Storytelling**

  + Polished the storytelling to be more coherent and engaging.

## The audience

The target audience is now narrowed down to Students, New York residents, frequent visitors, commuters, travelers, and drivers with a connection to New York since they can directly benefit from increased awareness of collision risks and safety precautions.

In my interview, I was suggested to provide specific solutions or recommendations. Therefore, I made some reflections on my story in order to talk about the "specific": my story is centered around the severity of the issue, the general pattern and facts, and the consequences, and is aimed at raising the awareness of people, so I think my target audience should not be those who are expertise in this area or those who are looking for specific related topics in terms of areas such as public health regarding road incidents. 

Realizing this, I modified my call-to-action section by discussing specific suggestions for my target audience based on the hourly, weekly, and seasonal patterns and the top contributing factors to vehicle collisions in New York, like *"remember the common threads that weave through these incidents: inattention, distraction, and unsafe driving behaviors. These are not just factors; they're choices. Choose to be part of the solution -- stay alert, respect traffic laws, and share this knowledge with fellow New Yorkers."*



## Final thoughts

In my final visualization, I narrowed down a lot of data to show and I found it unnecessary to expose readers to the full, wide range of data or trends across many years -- examples such as the modification of visualizations of *Average Proportion of Fatalities/injuries to Motorists, Pedestrians, and Cyclists* and *Weekly/seasonal collision variations*. It would be better to just include fewer years/ranges of data if they are already representive enough. Also, if there are similar patterns across different years -- in my case, the average proportions of injuries -- it would be better just to show this general result (I calculated the average in this case) while not including all the specific data -- people will be confused and it's hard for them to catch the main idea. In addition, it's important to visualize things that are important after analysis on my own while not just exposing everything to readers -- in my case, the original bad visualization of *Fatalities to Motorists, Pedestrians, and Cyclists* -- so that the narrative will have better focus and the visualizations can thus better serve the need of storytelling. Finally, the choice of different visualization designs is really important for readability. In my case, the area plot is way better than the bar chart when showing the *Weekly/seasonal collision variations*.
