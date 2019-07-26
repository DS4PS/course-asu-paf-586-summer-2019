---
layout: lab
title: Lab 04 - Feature Engineering 
image: microscope.png
---



<a class="uk-button uk-button-default" href="https://canvas.asu.edu/courses/26991/assignments/588320">Submit Lab 04</a>





## Overview

In the previous lab we examined the practice of feature selection - identifying the proper set of variables to use as inputs into a predictive model. Gottman developed a framework using 20 micro-expressions coded at one-second intervals. Iceland developed a set of variables that help predict whether teens are likely to abuse alcohol. 

A key pattern that emerges from the case studies and a take-away from Lab-03 is that identifying the proper data to include in a model is difficult. Typically experts will start with a large number of measures and eliminate variables as they are tested. It requires patience and attention to detail to identify the right set of variables for a given problem. 

This week we will explore the process of "feature engineering", the task of starting from raw data sources and "engineering" new variables by finding ways to code or extract new features. Unlike the second lab where researchers developed new instruments to measure specific latent constructs or hard-to-observe outcomes, feature engineering is common when using administrative dataset like satellite imagery, document archives, or video. It is common that the data was not designed for the task at hand, but it contains rich information that is extremely valuable if it can be extracted.

Feature engineering is also necessary because predictive models typically require quantitative variables, so data sources like images and text need to be transformed into counts and scales, similar to the variables you designed in the measurement labs. A large portion of efforts to build a new model typically entail figuring out how to "engineer" new variables from a raw data source. We cover several examples of what this process might look like below.

For example, how can a computer read handwriting? It has to be able to translate easily from an image of hand-written text to some sort of mathematical abstraction of the sentences. 

![](https://www.rsipvision.com/wp-content/uploads/2015/12/ocrpicss.jpg?w=450&ssl=1)

It accomplishes this by isolating words, then isolating individual characters, then using a pixel grid to code which features exist on each character (vertical lines, curved lines, cross-bars, etc.), and making a prediction about which letter it might be based upon specific features. 

<img src="https://cdn.mos.cms.futurecdn.net/FQhMbjgmQASC2EfezLXKub-1200-80.jpg" style="width:800px;">

*(Note, the elements above are concepts from typography that describe fonts, not a list of features from natural language processing, but you get the idea)*

Without a set of features extracted from the raw image of a character, the computer can't predict which letter it might be. In this way Lab-04 on Feature Engineering combines elements of Lab-02 on Measurement, and Lab-03 on Feature Selection. You "engineer" or "extract" a feature by first defining it (does the character possess a "bowl"), and then figuring out how the computer will observe or measure that feature. 

**Lab-02**: Training graduate students to code 20 different micro-expressions based upon body language and facial expressions is not that different from training a computer to code a specific feature. You need to first come up with a set of rules that will reliably identify each feature. Then write down the rules and see if others can follow them. The list of instructions for a grad student is similar to the list of instructions you will give a computer. No rule is perfect - some may work 95% of the time, some 80%, some 60%. In this way, the reliability of your rule for feature extraction is similar to the reliability of instruments you designed to observe latent constructs.

**Lab-03**: You could brainstorm hundreds of features that might be extracted from any raw data source. Some features will hold more information than others. Lots of letters have a verticle "stern" or a "loop", for example, but few have a "tail". Knowing that a character has a stern might cut your candidate pool in half, whereas knowing your character has a tail eliminates all but a couple of options. The goal is to identify features that are best able to differentiate between the outcomes you are trying to predict. Hopefully these features can be "engineered" from the raw input data with a decent level of reliability.

The goal of this lab is to demonstrate a couple of processes of feature engineering from common machine learning and artificial intelligence applications. I would like you to develop an intuitive sense of how engineers approach the creative endeavor of turning raw data into meaningful quantitative measures. Some steps below show how raw data might be processed to make it interpretable (to code characters from text, you first need to isolate individual characters). Others steps show how raw data is translated into a quantiative variable that can be used as an input into a model.

As you read through the lab, think about the readings from *Reality Mining* and *Social Physics*. How did computer scientists approach the task of understanding team performance in organizations? What sorts of [data did they collect](https://connection.mit.edu/human-strategy-0), and how did they generate quantitative measures from the raw data inputs of environmental sensors and employee smart badges? There are thousands of potential variables you could generate from human interactions in organizations, so how did they decide which measures were important? These themes will be revisited when we look at how Google tried to design the perfect team. 

We start here with some basic examples of feature engineering in a few task domains.


## Optical Character Recognition

The process by which computer programs read handwriting or scan images of text is quite interesting because of how raw image files are converted into structured data. The process is broadly called [Optical Character Recognition](https://blog.filestack.com/thoughts-and-knowledge/history-of-ocr/). [pdf](https://www.sciencedirect.com/science/article/pii/S2212671613000462)

<iframe width="400" height="315" src="https://www.youtube-nocookie.com/embed/bmTp-6lDQEA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br>

-------

<br>

For these tasks the program must first take an image and identify the different units of text:

![](http://www.dlib.org/dlib/july09/munoz/munoz-fig01.jpg)

These can then be broken into the most basic component parts, characters. The actual predictive models that comprise programs reading text occur on a letter by letter basis, and the paragraphs are reconstructed after all letters are identified:

![](https://miro.medium.com/max/1200/1*qBV12ANk-5epRv7231Zxzw.png)

For these programs to work the computer must be able to effectively isolate each character:

![](https://miro.medium.com/max/1400/1*IJyChJjetOLXowh4FzPQ1A.jpeg)

Images are a challenging data source because camera resolution, light sources, distance from the subject, and focus can all impact data quality. As a result, the first step in many applications that require computers to extract features from images is to process the image in a way that isolates the important information and standardizes some of the inputs.

Let's consider this basic program that allows you to take a picture of a graph, then will generate the underlying data for you. It does this by identifying the trend line, converting it to a pixel grid, then for each horizontal pixel measuring the vertical location of the trend line. 

Input image data can be messy, though. So first we need to standardize it to isolate the trend line. 

**Raw image of a graph**:

![](https://i0.wp.com/omnianalytics.io/wp-content/uploads/2019/06/line.jpg?w=450&ssl=1)

**Step 1**: Convert the colored picture to a grayscale version that emphasizes boundaries of graphics. 

![](https://i2.wp.com/omnianalytics.io/wp-content/uploads/2019/06/preview.png?w=450&ssl=1)

**Step 2**: Filter out any data that is below a threshold for opacity or darkness. 

![](https://i2.wp.com/omnianalytics.io/wp-content/uploads/2019/06/preview-2.png?w=450&ssl=1)

**Step 3**: Convert to a nagative view to maximize the contrast of the image. 

![](https://i1.wp.com/omnianalytics.io/wp-content/uploads/2019/06/preview-3.png?w=250&ssl=1)

The use of filters in this way is a common first step for models that use images as raw data sources. This will be true for self-driving vehicles that use cameras to collect data streams, or examples from the *Digital Humanitarians* text that use satellite images to predict the location of damage from a disaster. 

For an interesting urban policy application of this approach, thanks to an [program built by Microsoft](https://www.nytimes.com/interactive/2018/10/12/us/map-of-every-building-in-the-united-states.html
) you can now download a database of every single building in the United States that was built by an AI application that was taught to read satellite images.

<img src="https://static01.nyt.com/newsgraphics/2018/07/17/all-buildings-in-us/941536000c71273a13f8f5a891b1b2f1e316c136/tall-suburbs-mesa-800.jpg" style="width:800px;">

Let's look at how these techniques might be used to conduct a tree census.


## Trees

Trees are important for cities, but maintaining a robust urban forest is expensive and challenging. "Trees clean the air and water, reduce stormwater floods, improve building energy use, and mitigate climate change, among other things. For every dollar invested in planting, cities see an average $2.25 return on their investment each year." [cite](https://www.citylab.com/environment/2018/04/heres-how-much-money-trees-save-in-megacities/559211/)

If we want to moneyball trees in our city by bringing a data-driven approach to tree policy, we first need to measure out outcome. "How many trees are in your city? It might seem like a straightforward question, but finding the answer can be a monumental task. New York City’s 2015-2016 tree census, for example, took nearly two years (12,000 hours total) and more than 2,200 volunteers." [cite](https://www.citylab.com/environment/2018/12/urban-tree-canopy-maps-artificial-intelligence-descartes-labs/578701/)

Using high-resolution images that can capture a wide spectrum of light, data scientists have [designed ways to use public data sources and AI to perform this task](https://medium.com/descarteslabs-team/descartes-labs-urban-trees-tree-canopy-mapping-3b6c85c5c9cc). Here is a high-resolution image of Washington DC that has eliminated all of the light except that reflecting off of green objects, i.e. plant life in the city (as opposed to buildings and parking lots):

![](https://miro.medium.com/max/600/1*wIsDPFDS_B2wD1JeXB0k4A.gif)

Easy enough, right? But wait! Green patches might be grass, shrubs, or flowers. How does the program know to NOT count these green patches as trees?

![](assets/img/not-trees.png)

It turns out that trees reflect green light differently than other plants. If you apply the right filters you can further isolate the trees in the image from the rest of the plants. For example, watch the grass in the park disappear:

![](https://miro.medium.com/max/700/1*RqsTOuZbqbfH_yZCPCtcGQ.gif)

Or eliminate all of the open green spaces in Boston (the grass at the airport is especially vivid):

![](https://cdn.theatlantic.com/assets/media/img/posts/2018/12/Boston_tree_diff/390d37b06.gif)

These techniques allow us to isolate trees from everything else. But we now have another problem - a green island rarely contains a single tree. How can we isolate individual trees from a group of trees in a cluster? 

The nice [tutorial on tree canopy analysis](https://cran.r-project.org/web/packages/ForestTools/vignettes/treetopAnalysis.html) offers some solutions.

The basic recipe for identifying trees within a cluster is to:

**1. Apply a Filter** to isolate trees from other elements on the landscape.

<img src="/assets/img/lidar1.png" style="width:600px;">

**2. Detect Treetops** using [an algorithm](https://www.researchgate.net/publication/225076692_Seeing_the_Trees_in_the_Forest_Using_Lidar_and_Multispectral_Data_Fusion_with_Local_Filtering_and_Variable_Window_Size_for_Estimating_Tree_Height) that can predict the height of trees using information in Lidar images.

<img src="/assets/img/lidar2.png" style="width:600px;">

This step returns the geographic coordinates of each tree-top in the cluster so that you can see the tree through the forest.

Note that Lidar uses lasers to enhance typicaly digital photographic techniques by including rich measures of light frequency and the ability to triangulate height. Lidar is an expensive technology, but many cities (including Phoenix) have a database of Lidar images that are open for public use. 

**3. Model Canopies** 

<img src="/assets/img/lidar3.png" style="width:600px;">



![](/assets/img/lidar1.png)



## Faces


### Feature Extraction

The program will start with an image, and look for faces, frame the face, then look for prominent features so they can be isolated:

![](https://i.ytimg.com/vi/V7UdYzCMKvw/hqdefault.jpg)


Similar to the hand-writing recognition example, we can apply filters to an image to accentuate specific features. With letters on paper we are trying to maximize the contrast between the ink and the page. With faces, different filters applied to images (or image processing algorithms) will highlight specific facial features. 

![](https://media.springernature.com/original/springer-static/image/art%3A10.1007%2Fs13042-013-0182-4/MediaObjects/13042_2013_182_Fig5_HTML.jpg)

Once oriented to the face, an algorithm can identify facial landmarks that will be present on all faces: 

![](https://images.techhive.com/images/article/2014/02/facial_recognition-100245056-large.jpg)

The computer then translate the landmark view of a small set of prominent features to a grid model that measures the distance between each feature:

![](https://cdn-images-1.medium.com/max/1600/1*wh1N-kogDMaZYS17lqyqeQ.jpeg)

Voila! We now have a format that can be used to generate a quantitative variables describing a face. Each line represents a distance between facial landmarks. The length of each line becomes a distinct feature. 

You don't always know the distance from the camera to the face, so you might not be able to predict the actual size of specific features (is that person's nose large or was the camera just way too close?), but it is easy enough to calculate relative sizes. If you set the distance between the eyes to one, for example, then every other distance on this graph (each line) can be calculated relative to that distance. 

There are [many different ways](https://towardsdatascience.com/face-detection-for-beginners-e58e8f21aad9) to accomplish this basic process of creating abstract mathematical models of the face. They all return a list of quantitative features that describe an individual face.

And finally, we compare the measurements from a specific face against measurements in a large database of candidate faces. You can do this quickly because you are working with a few dozen measures (distance between eyes, distance between edges of the mouth, distance between edge of mouth to eye, etc.). You would calculate the difference between the face you are trying to identify, and each face in the database by comparing the length of each line. 

<img src="https://www.researchgate.net/profile/Abdullah_Al-Murad/publication/326682312/figure/fig1/AS:653988944957442@1532934523611/Face-recognition-workflow.png" style="width:800px;">


If the total distance between all of the features falls below a threshold, then the faces are flagged as a match to be examined further by a human, or some action is triggered (unlocking your phone or your front door, for example). 


<br>
 
 ------
 
### Feature Selection

Assuming that the photos are taken in good light with forward-facing subjects and decent resolution cameras, what do you anticipate being a challenge with this process? Facial feature landmarks might vary greatly based upon expressions (or angles of the camera):

![](https://www.mathworks.com/matlabcentral/mlc-downloads/downloads/submissions/45750/versions/1/screenshot.jpg)

Note that some features, like distance between the eyes and size of the nose, will be **static** (i.e. reliable measures). Others, like the edges of the mouth or the size of lips, will be **highly dependent upon the expression** (i.e. low alpha if we think about facial features as latent constructs). 

Stated another way, some features convey more information about the unique identity of an individual than others. The feature selection task is to identify which measures will contain the highest signal-to-noise ratios. The algorithms that match faces can also weight certain features more than others to account for expressions. 

[This paper](https://www.sciencedirect.com/science/article/pii/S0010027718302397) explores the issue by examining which facial features contain the most information during the recognition task. The do this by examing which features, when changed, render the individual most unrecognizable.

<img src="https://ars.els-cdn.com/content/image/1-s2.0-S0010027718302397-gr2_lrg.jpg" style="width:800px;">

Stated differently, if you omitted the high-salience features from your model like lip thickness, you would see a large drop in correct matches to the database. If you omit low-salience features like mouth size, you would experience a lower impact on the accuracy of facial recognition.

This example is meant to give you an intuitive sense of what the computer algorithm might experience as features are "corrupted" in the images, and remind you of the importance of the feature selection task.

So if you are trying to escape the country by crossing a border, which feature would you try to disguise? 

![](https://image1.masterfile.com/getImage/NjE5LTA1ODMyMzc0ZW4uMDAwMDAwMDA=AF4WWd/619-05832374en_Masterfile.jpg)







# Lab Questions:

## Part 1: Letters

Assume you have designed a program that can effectively isolate individual characters from an image of a license plate:

![](https://miro.medium.com/max/600/0*m2nX3yE5H8wik3rH.png)

You now want to develop a machine learning model that will accurately identify each character, so you need to develop a set of features that describe the letters so the computer can begin to tell them apart. 

List three features that could be reliably derived ("engineered") from an image of a single letter, and used as input data for a preditive model that can read the license plate accurately when the font used by states might vary.

![](http://dataaspirant.com/wp-content/uploads/2017/05/Mnist-database-hand-written-digits.png)

![](https://www.researchgate.net/profile/James_Landay/publication/221518120/figure/fig4/AS:668489102659594@1536391630464/Our-Digits-task-requires-recognition-of-handwritten-digits-Participants-collect-data.png)

If you think this sounds challenging, recognize that there are hundreds of potential features. Just look at how many terms hipsters have invented to lovingly diagram their favorite typefaces:

![](https://designmodo.com/wp-content/uploads/2011/08/typeface.jpg)

Or spend five minutes with a [hand-writing analyst](https://www.wikihow.com/Tell-What-Someone-is-Like-from-Their-Handwriting).

How would you describe the difference between these letters to a child? 

* You might start by pondering how someone would distinguish the difference between a lowercase "o" and a lowercase "a". 
* How would you describe the difference between a "1" and an "l"? 
* Between a zero "0" and an upper-case "O"?
* Capital "T" versus lower-case "t"? 


## Part 2: Professions

The blog **Toward Data Science** describes an interesting machine learning application that [predicts which category an object or person belongs to based upon an image](https://towardsdatascience.com/train-image-recognition-ai-with-5-lines-of-code-8ed0bdd8d9ba). They demonstrate the software by training it to guess a person's career based upon a picture of them at work:

> *For this tutorial, we have provided a dataset called IdenProf. IdenProf (Identifiable Professionals) is a dataset that contains 11,000 pictures of 10 different professionals that humans can see and recognize their jobs by their mode of dressing.*

![](https://miro.medium.com/max/700/1*BZB3eUcXb6atYuxJ6npVeQ.jpeg)

There are ten professions used in the example:

* Chef  
* Doctor 
* Engineer 
* Farmer 
* Firefighter 
* Judge 
* Mechanic 
* Pilot 
* Police 
* Waiter 

> *This dataset is split into 9000 (900 pictures for each profession) pictures to train the artificial intelligence model and 2000 (200 pictures for each profession) pictures to test the performance of the artificial intelligence model as it is training. IdenProf has been properly arranged and made ready for training your artificial intelligence model to recognize professionals by their mode of dressing. For reference purposes, if you are using your own image dataset, you must collect at least 500 pictures for each object or scene you want your artificial intelligence model to recognize.*

Suggest three features of uniforms that might be used to classify images from these professions. In this case, also include a rule statement about how you predict the feature to be used.

For example: 

* If the uniform has stripes on the arms, the individual will be a figherfighter or a pilot. 
* If the uniform includes a skirt the individual is not a farmer, mechanic, or chef (on the job). 
* If the uniform is mostly black, the individual will be a judge, pilot, or police officer. 
* If the uniform is mostly white, the individual will be a chef or a doctor.  
* If the uniform includes a bow tie, the individual will likely be a waiter (or an engineer?).  

![](https://miro.medium.com/max/420/1*kgFf3orScs_NwQyspLslAQ.jpeg)















---- 

<br>
<br>



<style>
img {
  width: 50%;
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
}
</style>

```
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
}
```
