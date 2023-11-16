| [Home Page](https://mingyu404.github.io/TellingStoriesWithData/) | [Visualizing Trust in News Organizations](/trust_news_organization.html) | [Visualizing Government Debt](https://mingyu404.github.io/TellingStoriesWithData/government_debt.md) | [Critique by Design](critique-by-design.md) | [Final Project I](final-project-part-one) | [Final Project II](final-project-part-two) | [Final Project III](final-project-part-three) |

# Critique of the Original Data Visualization

Original Data Visualization:  [Who Americans spend their time with, by age](https://ourworldindata.org/time-use#who-do-we-spend-time-with-across-our-lifetime)

<img width="817" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/5ee1be22-f505-4197-b716-88795755e037">

I selected this visualization for its engaging portrayal of a universal human experience — the allocation of our time. The interactive design provided a nuanced exploration of time spent with others across different ages, which I found innovative and deeply human.

## Pros:

- **Interactivity**:  The interactive design really helps compare different times with whom people spent given a specific age. 
- **Contextualization**:  The annotation/caption provides a good context for this visualization.

## Cons:

- **Color Scheme**: the colors chosen for "with friends" and "with coworkers" are quite similar, which makes it difficult for viewers to distinguish between the two lines at a glance. Also, the colors for “Alone” and “with coworkers” are red and green respectively, which is not friendly for some people to tell. 
- **Horizontal Axis Scaling**: the tick intervals in the horizontal axis are not consistent – the distance between the ages of 15 and 20 is not proportional to the distance between other age intervals of 10. 
- **Vertical Axis Scale**: the highest data points on the chart exceed the labeled y-axis values, potentially leaving viewers to estimate the precise figures. Although the interactive features can help reveal the exact data, it remains crucial for the chart's design to encompass extreme values on the axis for immediate clarity.
- **Title Ambiguity**: the title "by age" seems to indicate that age, in this case, is a categorical variable, but here is on the horizontal axis as a continuous variable, and the categories here are "alone", "with partner", etc. 

Overall, the above original design looks good to me, but there is still room for improvement. Prompted by these insights, I sketched a solution and sought feedback.

# Testing the Solution & Gathering Feedback

I presented the initial design to my friends, seeking their honest critiques. Here's what surfaced:

- **Student, mid-20s**: Suggested converting minutes to hours for an intuitive grasp of the data. This resonated with me as it aligns with the way we typically think about our day.
- **Student, mid-20s**: Recommended reducing vertical axis intervals for more granular and clear comparison. This feedback was pivotal, emphasizing the need for precision in visual data storytelling.
- **Student, mid-20s**: Pointed out including annotations in directing attention to key data points and trends. I found this to be a valuable insight, underscoring the role of annotations in enriching the narrative conveyed by data.

This feedback was invaluable. It not only validated some of my initial hunches but also shed light on aspects I hadn't considered.

# Building the Solution

With the insights from my audience, I embarked on a meticulous redesign:

1. **Time Conversion**: I converted minutes to hours, a more familiar time unit for daily reflection, ensuring the data resonated on a personal level.
2. **Color Scheme Modification**: I used a different color scheme to enhance readability and ensure that each category can easily stand out on its own.
3. **Refined Title**: The title was refined to encapsulate the data's essence while steering clear of any potential misinterpretation.
4. **Vertical Axis Adjustment**: The feedback on axis intervals was taken to heart, leading to smaller, more frequent markers, which allow for a more nuanced reading of the data. I also extended the axis to include values that cover the range of all data points presented.
5. **Horizontal Axis Standardization**: I changed the interval of the horizontal axis and made it uniform and linear.
6. **Data Annotations**: I added annotations near some critical data points, which can be useful for guiding the viewer's attention to important trends or critical turning points in the data. These annotations can provide context that isn't immediately apparent since there are many lines in the chart, making the visualization more informative and easier to understand.

Each modification was a deliberate step towards a visualization that not only informed but also connected with the general audience.

# Final Data Visualization

Here's the final redesign of the data visualization:

<div class='tableauPlaceholder' id='viz1700097348907' style='position: relative'><noscript><a href='#'><img
                alt='Social Time Distribution in the U.S.: Who Do People Spend Their Time with as They Age?Average time spent with others is measured in hours per day, and shown by the age of the respondent.This is based on averages from surveys between 2009 and 2019. '
                src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;hw&#47;hw34_17000972659030&#47;Sheet1&#47;1_rss.png'
                style='border: none' /></a></noscript><object class='tableauViz' style='display:none;'>
        <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
        <param name='embed_code_version' value='3' />
        <param name='site_root' value='' />
        <param name='name' value='hw34_17000972659030&#47;Sheet1' />
        <param name='tabs' value='no' />
        <param name='toolbar' value='yes' />
        <param name='static_image'
            value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;hw&#47;hw34_17000972659030&#47;Sheet1&#47;1.png' />
        <param name='animate_transition' value='yes' />
        <param name='display_static_image' value='yes' />
        <param name='display_spinner' value='yes' />
        <param name='display_overlay' value='yes' />
        <param name='display_count' value='yes' />
        <param name='language' value='en-US' />
        <param name='filter' value='publish=yes' />
    </object></div>
<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1700097348907'); 
    var vizElement = divElement.getElementsByTagName('object')[0]; 
    vizElement.style.width = '100%'; 
    vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px'; 
    var scriptElement = document.createElement('script'); 
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; 
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

I maintained the line chart representation from the original version, as its capacity to compare trends across various social interactions over time was effective and meaningful. The line graph format naturally lends itself to depicting the fluid nature of time and the gradual shifts in social habits, which is central to the story being told by the data.

I sought not to reinvent but to refine, enhancing the existing strengths of the visualization. For instance, the annotations I introduced serve to highlight key transitions and trends, such as the increase in alone time starting in the 40s and the decline in coworker interaction after retirement in the mid-60s. These notes act as signposts, guiding the viewer through the data's narrative arc and emphasizing the significant moments that collectively chart the course of American social life.

In general, the final redesign of the data visualization, "Social Time Distribution in the U.S.: Who Do People Spend Their Time with as They Age?", presents a more intuitive and insightful exploration of the changing social dynamics across different life stages by applying the modifications mentioned in [Building the Solution ](#Building the Solution)section. My focus was on amplifying clarity, enriching context, and improving the overall visualization quality. The new visualization not only provides information but also strikes a chord with viewers on an individual level, prompting them to contemplate their own social journeys.
