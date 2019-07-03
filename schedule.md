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

* Lewis, M. (2018). The Fifth Risk. WW Norton & Company. CH5: all the president’s data pp 148-179
* [The Age of Big Data: New York Times](https://www.nytimes.com/2012/02/12/sunday-review/big-datas-impact-in-the-world.html) 

> How much did Friedberg pay for the NOAA weather data? How much did his company sell for? What is the economic value of government data?






*** { @unit = "", @title = "Open Data (Team 1)", @reading, @foldout }

# Open Data

* Eagle, N., & Greene, K. (2014). Reality mining: Using big data to engineer a better world. MIT Press. **CH7 mobile and internet data**
* Lewis, M. (2018). The Fifth Risk. WW Norton & Company. CH5: data as a public good pp **148-179**

> The value of public data will often be unlocked by private individuals or firms. What is the difference between Friedberg’s use of NOAA data and AcuWeather’s use of the data? 


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

This week's lab will introduce you to two data-driven models of neighborhood change. We will use this case study over the next six weeks to discuss things like data needs for predictive models. You will be required to think critically about the data used in the labs, but you will not be responsible for things like the advanced analytical models in the paper. I am approaching the labs with the assumption that you are likely to be a manager hiring an analyst, so you need a high-level understanding of the models in order to find someone for the task. 

Read the following chapter and paper:

Market Value Analysis: A Data-Based Approach to Understanding Urban Housing Markets. pp 49-59 [ [PDF](https://github.com/DS4PS/paf-586-summer-2019/raw/master/Reading/MVA-DD-App-to-Strengthening-Neighborhoods.pdf) ]

Delmelle, E. C. (2017). Differentiating pathways of neighborhood change in 50 US metropolitan areas. Environment and planning A, 49(10), 2402-2424. [ [PDF](https://github.com/DS4PS/paf-586-summer-2019/raw/master/Reading/differentiating-pathways-of-neighborhood-change.pdf) ]

### We are interesting in understanding neighborhood change. How did each author identify coherent "neighborhoods" (or groups) in each model? Did they use the same data to create the groups? How do the descriptions of the groups differ?  





** Week 2 - Collecting Data


*** { @unit = "1st April", @title = "Intro to Data-Driven Management and Policy", @reading, @lecture, @assignment, @foldout }

# Topics

* Introduction to the course
* Overview of R, R Studio, and Markdown,
* Uses of data in public management


# Readings

### Required

Textbook: [Chapter 1](https://ds4ps.org/Data-Science-Class/TEXTBOOK/docs/introduction-to-r.html)

[R Markdown: The bigger picture - Garrett Grolemund](https://resources.rstudio.com/rstudio-conf-2019/r-markdown-the-bigger-picture)

[Markdown Basics](https://ds4ps.github.io/data-driven-management-textbook/markdown/)

### Suggested

[The Promise of Big Data ](https://www.theregister.co.uk/2017/06/07/go_small_on_big_data/)

[Go Small on Big Data](https://www.theregister.co.uk/2017/06/07/go_small_on_big_data/)

[Becoming a Data Drive Org](https://sloanreview.mit.edu/case-study/lessons-from-becoming-a-data-driven-organization/)

# Lab

[Overview](labs/Lab_01_Overview_and_Example.html)

[Template](labs/Lab-01-Template.Rmd)


# Class Examples

[Powerpoint](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Lecture%2001%20-%20Introduction%20to%20the%20Class.pptx)

[Recording of Lecture](https://asu.zoom.us/recording/play/EKu_Dv5Gp7k452S5v5y_o_pYEKuHUNPpn7FT0yoHW2M3-rcrd5wN1nOaU_n1XWqq?continueMode=true)


** Section-II Data Programming



*** { @unit = "8th April", @title = "R Basics", @reading, @lecture, @assignment, @foldout }

# Topics

* Data types in R
* Ways  of  collecting  data:  passive,  active,  administrative  intro  to  life  logging  and  semester project.
* Design of Experiments.

# Readings

### Required

[Getting Started on Quantified Life](https://quantifiedself.com/get-started/)

[Reality Mining](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Reality_Mining_Chapter%201pdf.pdf)

[TED - What to Do With Big Data](https://www.ted.com/talks/susan_etlinger_what_do_we_do_with_all_this_big_data)

[Managerial Experiments](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Appendix%20A%20-%20Experiment%20Design%20(1).pdf)

### Suggested

[Challenges of Harnessing Data](https://sloanreview.mit.edu/case-study/lessons-from-becoming-a-data-driven-organization/)

[Abundant Data by Itself Solves Nothing ](https://graymattersystems.com/cio-survey-reveals-challenges-opportunities-potential-industrial-big-data/)

[Big Data: The Management Revolution](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Big%20Data_%20The%20Management%20Revolution.pdf)

[Building a Learning Organization](https://hbr.org/1993/07/building-a-learning-organization)

# Lab

[Lab for Homework](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Lab%2002%20Template.Rmd)

# Class Examples

[In Class Work](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/In%20Class%202.Rmd)

[Recording of Lecture](https://asu.zoom.us/recording/share/xiGjNWxnP33Y4xIjbacyfFtMOABFywTfFfquD3urC1E?startTime=1554767802000)

[Powerpoint](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Lecture%2002%20-%20Intrroduction%20to%20Experiments.pptx)


*** { @unit = "15th April", @title = "Data Structures in R", @reading, @lecture, @assignment, @foldout }

# Topics

* Lists 
* Vectors 
* Data frames 

# Readings

### Required

Textbook: [Chapter 2-3](https://ds4ps.org/Data-Science-Class/TEXTBOOK/docs/data-types.html)

### Suggested

[Data Sources from Lab 2](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Lab%20Assignment%202%20Data%20Sources.pdf)

# Lab

[Lab for Homework](https://escience.washington.edu/wp-content/uploads/2019/04/Session3_DataStructures_LAB.html)

# Class Examples
<a href="https://escience.washington.edu/wp-content/uploads/2019/04/Session3_DataStructures.html" target="_blank">Lesson code</a>

<br>
* [download ALL files for session 3](https://github.com/EvansDataScience/DataDriven_ManagementAndPolicy/raw/master/Session3.zip)

[Recording of Lecture](https://asu.zoom.us/recording/share/QZZRh26ZkHz4KYkKbm5QLGrpUWmBsz-UQGd_p_N5t0-wIumekTziMw)


*** { @unit = "22th April", @title = "Working with Data Frames", @reading, @lecture, @assignment, @foldout }

# Topics

* Logical operators
* Control of execution
* Functions

# Readings

### Required

Textbook: [Chapter 4-8](https://ds4ps.org/Data-Science-Class/TEXTBOOK/docs/logical-statements.html)


### Suggested

# Lab

[Lab for Homework](https://escience.washington.edu/wp-content/uploads/2019/04/session4_LAB.html)



# Class Examples

<a href="https://escience.washington.edu/wp-content/uploads/2019/04/session4_DataFrame.html" target="_blank">Lesson code</a>


* [download ALL files for session 4](https://github.com/EvansDataScience/DataDriven_ManagementAndPolicy/raw/master/session4.zip)

[Recording of Class](https://asu.zoom.us/recording/share/UzY4YVDixOsmkCU5LlA7JqVNpZuT0f6jfg8ICmtwaquwIumekTziMw)

*** { @unit = "29th April", @title = "Intro to Visualization", @reading, @lecture, @assignment, @foldout }

# Topics

* Visualization guidelines 
* R and the grammar of graphics 

# Readings

### Required

Textbook: [Chapter 9-11](https://ds4ps.org/Data-Science-Class/TEXTBOOK/docs/the-plot-function.html)


### Suggested

# Lab

[Lab for Homework](https://escience.washington.edu/wp-content/uploads/2019/04/session5_LAB.html)

# Class Examples

<a href="https://escience.washington.edu/wp-content/uploads/2019/04/session5.html" target="_blank">Lesson code</a>


* [download ALL files for session 5](https://github.com/EvansDataScience/DataDriven_ManagementAndPolicy/raw/master/session5.zip)

[Recording of Class](https://asu.zoom.us/recording/share/RCc1y6K9rxrpaGMCGjaFw21QNxTvgq3yo3JnMYC0enKwIumekTziMw)

*** { @unit = "6th May", @title = "Spatial and Multidimensional visualization", @reading, @lecture, @assignment, @foldout }

# Topics

* Bivariate and multivariate plots
* Mapping in R

# Readings

### Required

### Suggested

# Lab

[Lab for Homework](https://escience.washington.edu/wp-content/uploads/2019/05/session6_LAB.html)

# Class Examples

<a href="https://escience.washington.edu/wp-content/uploads/2019/05/session6.html" target="_blank">Lesson code</a>

* [download ALL files for session 6](https://github.com/EvansDataScience/DataDriven_ManagementAndPolicy/raw/master/Session6.zip)

[Recording of Class](https://asu.zoom.us/recording/share/kwJpBI7xSdOi-ozjvnOEaTxqoL4G1EQ5TVSBf9oDHnewIumekTziMw)

** Section-III Dashboards

*** { @unit = "13th May", @title = "Dynamic visualization", @reading, @lecture, @assignment, @foldout }

# Topics

* The design and construction of dashboards.

# Readings

### Required

[Flexdashboard Tutorial](https://rmarkdown.rstudio.com/flexdashboard/)

### Suggested

[History of Urban Dashboards](https://placesjournal.org/article/mission-control-a-history-of-the-urban-dashboard/?cn-reloaded=1)

[Laws of Shitty Dashboards](http://attackwithnumbers.com/the-laws-of-shitty-dashboard)

# Lab

[Lab 7 HTML](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Lab_7.html)

[Lab 7 RMD](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Lab%207.Rmd)

[Starting Dashboard](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Pets_Dashboard.html)

[Data](https://data.seattle.gov/Community/Seattle-Pet-Licenses/jguv-t9rb)

# Class Examples

[Recording of Lecture](https://asu.zoom.us/recording/share/qVs7I0HsMn5YNRqNXfb7hfAY9gNYujb56KAW10GVQ46wIumekTziMw)

*** { @unit = "20th May", @title = "Analyzing Managerial Experiments", @reading, @lecture, @assignment, @foldout }

# Topics

* Analysis of experiments
* Testing outcomes in R

# Readings

### Required

[Interrupted Time Series](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Interrupted%20Time%20Series.pdf)

### Suggested

# Lab

[Lab 8](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Lab%208.Rmd)

# Class Examples

[Class Example - Eric Sleep](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Lecture%208.Rmd)

[Recording of Lecture](https://asu.zoom.us/recording/share/AZRAxmSQ21eD7L7gLlDGiBLW8jSTztLkylB3vggIqnWwIumekTziMw)

*** { @unit = "27th May", @title = "MEMORIAL DAY" }

# No Classs

Instructions will be given on what to do for this week.




*** { @unit = "3rd June", @title = "Dashboards II", @reading, @lecture, @assignment, @foldout }

# Topics

* Shiny widgets.
* Advanced dashboards.

# Readings

### Required

### Suggested

[Building Shiny Apps Guide](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Building%20Shiny%20apps%20-%20an%20interactive%20tutorial.pdf

[Shiny App Layout](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Shiny%20-%20Application%20layout%20guide.pdf)

# Lab

[Lab 09](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Lab%209.Rmd)

# Class Examples

[Lecture Notes](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/Reading/Intro%20to%20Shiny.pdf)

Those notes, by virtue of being printed to add to the website, will not be dynamic. If you want to experiment with the sliders and other features, copy the code into R and run with the shiny package.

[Lecture Recording](https://youtu.be/JvJe5mljql8)

The lecture was uploaded to YouTube. This is my first time doing that, so please let me know if there are any technical issues.

*** { @unit = "11th June", @title = "FINAL PROJECTS DUE", @assignment, @foldout }

# Instructions

There are two components of the final project, both of which must be completed seperately: the data repository and the dashboard. Instructions for both are below.

[Instructions for Data Repository](http://rpubs.com/evanholm/499103)

[Instructions for Dashboard](https://github.com/DS4PS/ddmp-uw-class-spring-2019/blob/master/labs/Dashboard%20Overview.Rmd)








***  


