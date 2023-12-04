| [Home Page](https://mingyu404.github.io/TellingStoriesWithData/) | [Visualizing Trust in News Organizations](/trust_news_organization.html) | [Visualizing Government Debt](/government_debt.md) | [Critique by Design](critique-by-design) | [Final Project I](final-project-part-one) | [Final Project II](final-project-part-two) | [Final Project III](final-project-part-three) |

# Introduction

### Topic

Navigating the Risks: A Data-Driven Look at New York's Vehicle Collisions

### Intro

Across the bustling expanse of New York, traffic accidents are an all-too-common part of the cityscape, with a substantial number leading to critical injuries and loss of life. This persistent issue is highlighted by the New York State Department of Health, which reports motor vehicle accidents as the leading cause of injury-related deaths in the state ([Car Accident Facts and Figures](https://www.scottgottlieblaw.com/car-accident-lawyer/facts-figures/), 2021). Although the [data](https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes) from recent years indicates a downward trend in collision numbers, the injuries and fatalities remain distressingly high. In the year 2022 alone, 51,928 New Yorkers were injured and nearly 300 lives were lost due to vehicular accidents. An examination of over two million collision records paints a  picture of these incidents, revealing the daily risks and the imperative for safer travel narratives throughout New York.

### Dataset

The data is found at: [https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes](https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes)

Since the original data has a lot of N/A values in some columns and repetitive fields, I did some data cleaning and initial EDA to get the new filtered dataset, adding additional variables for more efficient analysis and visualization. 

Here is part of the process of data processing with Python.

<img width="759" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/866796f3-fc8e-489b-b181-5a87360909a6">

Here is the basic information about the filtered dataset.

```
motor_vehicle_collision_filtered.info()

<class 'pandas.core.frame.DataFrame'>
RangeIndex: 2043611 entries, 0 to 2043610
Data columns (total 28 columns):
 #   Column                         Dtype         
---  ------                         -----         
 0   CRASH DATE                     datetime64[ns]
 1   CRASH TIME                     object        
 2   BOROUGH                        object        
 3   ZIP CODE                       object        
 4   LATITUDE                       float64       
 5   LONGITUDE                      float64       
 6   LOCATION                       object        
 7   ON STREET NAME                 object        
 8   CROSS STREET NAME              object        
 9   NUMBER OF PERSONS INJURED      float64       
 10  NUMBER OF PERSONS KILLED       float64       
 11  NUMBER OF PEDESTRIANS INJURED  int64         
 12  NUMBER OF PEDESTRIANS KILLED   int64         
 13  NUMBER OF CYCLIST INJURED      int64         
 14  NUMBER OF CYCLIST KILLED       int64         
 15  NUMBER OF MOTORIST INJURED     int64         
 16  NUMBER OF MOTORIST KILLED      int64         
 17  CONTRIBUTING FACTOR VEHICLE 1  object        
 18  CONTRIBUTING FACTOR VEHICLE 2  object        
 19  COLLISION_ID                   int64         
 20  VEHICLE TYPE CODE 1            object        
 21  VEHICLE TYPE CODE 2            object        
 22  CRASH YEAR                     int64         
 23  CRASH MONTH                    int64         
 24  CRASH MONTH NAME               object        
 25  CRASH HOUR                     int64         
 26  CRASH WEEK                     object        
 27  CRASH SEASON                   object        
dtypes: datetime64[ns](1), float64(4), int64(10), object(13)
memory usage: 436.6+ MB
```

Complete filtered dataset used in this project can be found at [filtered data](https://drive.google.com/file/d/12FEnHLSqzG-Lvxcs3yNbyBPDKON6DXkr/view?usp=drive_link). The data cannot be uploaded to the Github repository since it is too large.

I will explore the relationships among these variables to figure out the pattern of collision numbers by year, region, season, hour, etc. The following is my outline that details how I will use this dataset.

# Outline

## Background introduction

### Yearly overview
Present a visual comparison of yearly collision numbers against injuries and fatalities from 2012 to 2022. Highlight the disparity between the declining collision numbers and the stubbornly high casualty figures -- each crash now seems to have more serious consequences than the previous one. 

<img width="751" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/f5705a23-ddce-4189-9fde-ef4d9585f37b">
<img width="742" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/9778b732-8f4e-43f1-a8b0-65aa7f9ee2ea">

### Regional analysis

Use a map to illustrate collision hotspots in New York. Discuss the frequency of accidents in different regions and highlight the most dangerous streets and intersections.

**2012 collisions by region**

<img width="756" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/ba91e23b-1e57-4dc9-a7a5-327050df919a">

**2022 collisions by region**

<img width="756" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/a93e1719-2323-4266-97e8-6b5c4d2e8aa3">

>Collisions are more frequent on Manhattan Island, with an increasing frequency of collisions from 2012 through 2022.

**The most dangerous street where collisions happen most in recent 5 years**

<img width="756" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/b9528cdc-be52-419e-8521-026e0332b7b5">

## **Collision Patterns**

### Hourly distribution

Provide a visualization showing collision frequency by hour. Emphasize the risks associated with rush hours and the relative calm of the late-night hours.

<img width="745" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/0e7290c3-ca00-4e43-9934-6814ec388729">

### Daily dynamics

Display a visualization of collision numbers by weekday: starting Monday, collision numbers rise, peaking on Friday, followed by a weekend decline. Discuss possible reasons for this pattern.

<img width="751" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/8e93fb67-e740-4d03-a073-47c3fcb8961c">

### Seasonal variations

Display the seasonal pattern of collision numbers: more frequent collisions in summer and fall while less frequent collisions in winter, noting the anomaly of the 2020-21 season.

<img width="752" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/3d2f0844-271b-4243-b197-7ba109407fba">

### Collisions by vehicle types

List visualization of top vehicles most frequently involved in collisions and discuss any patterns or surprises in this data.

<img width="758" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/08a23f94-4bb4-4360-83ac-c01a4a538e44">

> The top 6 vehicle types most freqeunty associated with car accidents are Station wagon / sport unitility vehicle, sedan, passanger vehicle, taxi, pick-up taxi, and van.


<img width="754" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/ee0a56b2-db77-4e59-9da9-751375b8d349">

> Of these six major vehicle types, sedans and station wagons/sport utility vehicles were the ones involved in the most crashes over the past six years.

## Causes

Explore top factors contributing to collisions.

<img width="754" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/833d2ec5-2f01-42ee-aa7f-5a49c1f9cf9d">

Will also include some news and reports from other sources to make the discussion more intuitive in this part. e.g. [Car Accident Facts and Figures](https://www.scottgottlieblaw.com/car-accident-lawyer/facts-figures/).

## Consequences -- the human cost

Present the numbers of injured and killed in a clear format. Break down these figures into pedestrians, cyclists, and motorists to highlight the varying degrees of vulnerability.

**Number of people injured**

<img width="751" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/fdc990cc-181a-4282-a937-eac44a192573">

**Number of people killed**

<img width="750" alt="image" src="https://github.com/mingyu404/TellingStoriesWithData/assets/123033972/f556c4e6-d9db-40a3-b1b3-caf2ee8f93ef">


## Conclusion & Call to action

The analysis navigated the when, where, and how of New York's vehicle collisions. The patterns uncovered are not mere statistics—they're calls for heightened awareness and preventative action. 

Data informs change. Let this analysis be a catalyst for enhanced safety measures, targeted education, and impactful policy reforms, steering towards a future where New York's streets are not just vibrant, but also safer for all.

# Method and medium
I will be using Shorthand to create the story of a vehicle collision in New York, which will include all of my finalized visualization works using Tableau, Canva, and probably Figma.
