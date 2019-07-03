---
layout: schedule
title: Schedule
---
 
<!--- 
New sections start with 2 stars:  ** Section Title
New units start with 3 stars:     *** {Unit Metadata}
-----------------------------start example
** Section-I
*** { @unit = "15th Nov", @title = "Course Overview", @reading, @lecture, @assignment, @foldout }
-----------------------------end example
Unit Metadata is comprised of:
@unit - date or number
@title - unit name
@reading - turn on reading icon
@assignment - turn on lecture icon
@lecture - turn on lecture icon
@foldout - activate unit content (allow foldout)
-->



** Week 1


*** { @unit = "July 7th", @title = "The Value of Data", @reading, @foldout }


# The Value of Data

* [The Age of Big Data: New York Times](https://www.nytimes.com/2012/02/12/sunday-review/big-datas-impact-in-the-world.html) 
* Lewis, M. (2018). The Fifth Risk. WW Norton & Company. **CH5: all the president’s data pp 179-188** [ [PDF](https://github.com/DS4PS/paf-586-summer-2019/raw/master/Reading/fifth-risk-CH5-all-the-presidents-data.pdf) ] 

How much did Friedberg pay for the NOAA weather data? How much did his company sell for? What is the economic value of government data?

<br>
<br>




*** { @unit = "", @title = "Open Data (Team 1)", @reading, @foldout }

# Open Data

* Eagle, N., & Greene, K. (2014). Reality mining: Using big data to engineer a better world. MIT Press. **CH7 mobile and internet data**
* Lewis, M. (2018). The Fifth Risk. WW Norton & Company. CH5: data as a public good pp **148-179** [ [PDF](https://github.com/DS4PS/paf-586-summer-2019/raw/master/Reading/fifth-risk-CH5-all-the-presidents-data.pdf) ] 

The value of public data will often be unlocked by private individuals or firms. What is the difference between Friedberg’s use of NOAA data and AcuWeather’s use of the data? 


*** { @unit = "", @title = "The Big Promise of Big Data (Team 2)", @reading, @foldout }

# The Big Promise of Big Data

* Pentland, A. (2015). Social Physics: How social networks can make us smarter. Penguin. **CH1**
* Meier, P. (2015). Digital humanitarians: how big data is changing the face of humanitarian response. Routledge. **CH1**


*** { @unit = "", @title = "Challenges of Big Data (Team 3)", @reading, @foldout }

# Challenges of Big Data (Team 3)

* O'Neil, C. (2016). Weapons of math destruction: How big data increases inequality and threatens democracy. Broadway Books. **Introduction pp 1-13**  
* [Desouza, K. C., & Smith, K. L. (2014). Big data for social innovation. Stanford Social Innovation Review, 2014, 39-43.](https://ssir.org/articles/entry/big_data_for_social_innovation#)  
* Duhigg, C. (2016). Smarter faster better: The secrets of being productive. Random House. **CH8 pp 238-247, 252-267**  



*** { @unit = "July 9th", @title = "LAB 1: Models of Neighborhood Change", @assignment, @foldout }

# Week 1 Lab

This week’s lab will introduce you to two data-driven models of neighborhood change. We will use this case study over the next six weeks to discuss things like data needs for predictive models. You will be required to think critically about the data used in the labs, but you will not be responsible for things like the advanced analytical models in the paper. I am approaching the labs with the assumption that you are likely to be a manager hiring an analyst, so you need a high-level understanding of the models in order to find someone for the task.

Neighborhood change is a complicated concept with a lot of loaded terminology. We might think about neighborhoods that are "revitalized", "gentrified", that are "stable", or that "decline".  We could spend an entire semester unpacking all of these constructs, but that is out of scope of the lab. Here we are more interested in how we might make sense of our data, and then once we have meaningful groups how we might use them to make predictions with the data. Can a city forecast how it's current neighborhoods are likely to change over the next decade, and can that help with urban planning processes? 

Read the following articles:

Market Value Analysis: A Data-Based Approach to Understanding Urban Housing Markets. pp 49-59 [ [PDF](https://github.com/DS4PS/paf-586-summer-2019/raw/master/Reading/MVA-DD-App-to-Strengthening-Neighborhoods.pdf) ]

Delmelle, E. C. (2017). Differentiating pathways of neighborhood change in 50 US metropolitan areas. Environment and planning A, 49(10), 2402-2424. [ [PDF](https://github.com/DS4PS/paf-586-summer-2019/raw/master/Reading/differentiating-pathways-of-neighborhood-change.pdf) ]

We are interesting in understanding neighborhood change. These data-driven approaches to the phenomenon use machine-learning algorithms to "discover" coherent communities within the city by grouping census tracks into groups that minimize within-group differences and maximize between-group differences. 

You can explore one of these algorithms by looking at examples of how botanists might create "species" based upon characteristics of flowers:

[Clustering Example](https://shiny.rstudio.com/gallery/kmeans-example.html)

A data-driven approach to understanding neighborhood change requires use to (1) define "neighborhoods", or groups of census tracks in the data that are very similar, and (2) use those group characteristics at a point in time to predict how they "neighborhood" might change in the future. Both of the papers present variations on Step (1) above.

Read the two papers, then answer the following questions:

1. **How did each author identify coherent “neighborhoods” (or groups) in each model?**
2. **Would these "neighborhoods" line up with neighborhoods that are defined on a city's zoning maps (Links to an external site.)?**
3. **Did the two models use the same data to create the groups?**
4. **How do the labels and descriptions of the groups differ in each model and why?**

Write your responses in a word document, save your responses as a PDF and name your file LAB-01-YOUR-LAST-NAME.pdf, then submit it via the Canvas assignment tool. 

Concise and precise answers are preferred to meandering paragraphs! One page would be fine for this assignment. 

Submit your lab through the [Canvas Shell](https://asu.instructure.com/courses/26991/assignments/572663).





** Week 2 - Collecting Data


*** { @unit = "July 14th", @title = "Data on Teams (Team 4)", @reading }

*** { @unit = "", @title = "Eyes in the Sky (Team 5)", @reading }

*** { @unit = "", @title = "Social Media Data (Team 1)", @reading }

*** { @unit = "", @title = "Remote Sensors (Team 2)", @reading }

*** { @unit = "July 17th", @title = "LAB 2 - Variables and Measurement", @assignment }


** Week 3 - Prediction  

** Week 4 - Challenges of Big Data

** Week 5 - Managing with Data 

** Week 6 - Data-Driven Human Resources  





