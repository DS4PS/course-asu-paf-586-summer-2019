---
layout: lab
title: Lab 03 - Feature Selection 
image: microscope.png
---



<a class="uk-button uk-button-default" href="https://canvas.asu.edu/courses/26991/assignments/588320">Submit Lab 03</a>



How many trees are in your city? It might seem like a straightforward question, but finding the answer can be a monumental task. New York City’s 2015-2016 tree census, for example, took nearly two years (12,000 hours total) and more than 2,200 volunteers.

https://www.citylab.com/environment/2018/12/urban-tree-canopy-maps-artificial-intelligence-descartes-labs/578701/

My research team has calculated just how much a tree matters for many urban areas, particularly megacities. Trees clean the air and water, reduce stormwater floods, improve building energy use, and mitigate climate change, among other things. For every dollar invested in planting, cities see an average $2.25 return on their investment each year.

https://www.citylab.com/environment/2018/04/heres-how-much-money-trees-save-in-megacities/559211/


## Overview

![](https://www.rsipvision.com/wp-content/uploads/2015/12/ocrpicss.jpg?w=450&ssl=1)


![](https://i0.wp.com/omnianalytics.io/wp-content/uploads/2019/06/line.jpg?w=450&ssl=1)

![](https://i2.wp.com/omnianalytics.io/wp-content/uploads/2019/06/preview.png?w=450&ssl=1)

![](https://i2.wp.com/omnianalytics.io/wp-content/uploads/2019/06/preview-2.png?w=450&ssl=1)

![](https://i1.wp.com/omnianalytics.io/wp-content/uploads/2019/06/preview-3.png?w=250&ssl=1)


<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/bmTp-6lDQEA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



![]()

[pdf](https://pdf.sciencedirectassets.com/282179/1-s2.0-S2212671613X00022/1-s2.0-S2212671613000462/main.pdf?X-Amz-Security-Token=AgoJb3JpZ2luX2VjEKP%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIQCcsi6pLBE5NGwr5ggO8dwNYEtwFw9AB3Y2dl2lNhJA%2FAIgG6YcusRapQjClJg7tXT55vB45qLIz%2BXS1IcpqgAv4HUq2gMIHBACGgwwNTkwMDM1NDY4NjUiDLkrq3e1S10FMCilbCq3Ayi5At%2FtK1TiMxn9Xge%2BuPEjP2OJ6%2B9LyKvu%2Bq6T3LUQGc10s0XXGRXhfOEwPtOQzvGtIHk%2Bcme0nzyqMik3ro6PE%2BjmLNvnQgzNul5iCXLDg8zlb8ki1Q%2Fy2txcXcw9RDcLyis%2Fw9nHnn2DWXZvEM5VuK6uWOFqtAPNK3kW0Hk2nfS2Ia6qhN4pm5f2CcdVB9UE4erMSrxf3Di8VanMtyjw91mRkwVijxfFo0N0fJcYOk6PtRzGDn6tS6no51sQrgIUKOtWBwYSs6b4zve4POZuvAE5upp6sONwxseIwNZq1ScUlgVwABgdGqLZKns2PkFS7iD%2BKhBqofK8XhYxZfOo2j7EYzb1%2FTqMZZSd%2BiFIQbhdIsOv1gFZ8oE%2B0jaFVz0kl6gL%2BYGJPjb5w2qtdKfz11Lsh4htsqZehGVzm1g0zCX7gA8AUCZphFJ%2F34fWHtJLJ8ryF2CaNY5rMC6vBKCMA%2Fk3vqGaqWMHsZi%2Fkae5zH%2BNVOoAKoJavwaBJvDHLh6dyb9qaUY38h3B8PktgcGJvf0G2XADa7%2F05nL3Q5OBtu4rkl4sfBGGUirPEDlOYRXdj64gf4Ywnenn6QU6tAEbYpLzETUW87tNgh%2Bg2M8LLelNtlqTdYWSvi90HXpm%2BLMeoLqpaX78iJMTVn107otw0BjQAlLxRD5D5bcShft96i8H5Ua4PoVgR26H3yAPnPr9V8D2qQGgwK9XGZukIMfpR%2Bep3ym7l0s7Mw2wC1l4XNmURI2n5iYE2aYLF44wgVVb%2BWgDER7D1SD0mVZRcCWe4M5npFgc%2FGa1Q%2BEgRs5zB6M7ZwDB9fa9JsW%2FNrbGmRZ44gU%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20190725T201702Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY2RCAY2UX%2F20190725%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=af30e4f66333913bf93a7253f07046523f047994738c265963a4ce22dc4d4d57&hash=781e3752e7512680b664b1e572552d5029c9539225e5d461d6e07aac0a199ad9&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S2212671613000462&tid=spdf-ee4668c8-e1a3-4845-9b9e-172aea53f6ad&sid=1cb538e639f0c84e2559dfa-914f5c91fbc1gxrqa&type=client)



## Pronouns

![](http://www.dlib.org/dlib/july09/munoz/munoz-fig01.jpg)

![](https://www.yourdictionary.com/image/articles/18831.partsSpeech.jpg)




## Faces

![](https://ars.els-cdn.com/content/image/1-s2.0-S0010027718302397-gr2_lrg.jpg)


Similar to the hand-writing recognition example, we can apply filters to an image to accentuate specific features. With letters on paper we are trying to maximize the contrast between the ink and the page. With faces, different filters applied to images (or image processing algorithms) will highlight specific facial features. 

![](https://docs.opencv.org/2.4/_images/eigenfaces_opencv.png)
![](https://media.springernature.com/original/springer-static/image/art%3A10.1007%2Fs13042-013-0182-4/MediaObjects/13042_2013_182_Fig5_HTML.jpg)

The program will start with an image, and look for faces, frame the face, then look for prominent features so they can be isolated:

![](https://i.ytimg.com/vi/V7UdYzCMKvw/hqdefault.jpg)

Once oriented to the face, an algorithm can identify facial landmarks that all people share: 

![](https://images.techhive.com/images/article/2014/02/facial_recognition-100245056-large.jpg)

We can then move from the landmark view to an abstract model of the face:

![](https://miro.medium.com/max/1838/1*qh_cSRND5RdS8g_U_r3F2A.jpeg)

Voila. We now have a mathematical model that can be used to generate a quantitative dataset from the face. You don't always know the distance from the camera to the face, so you might not be able to predict the actual size of specific features (is the face actually large or was the camera just way too close?), but it is easy enough to calculate relative sizes. If you set the distance between the eyes to a one, for example, then every other distance on this graph (each line) can be calculated relative to that distance. Each line on this image then represents a separate "feature", or data point in the database. 

![](https://www.risk-uk.com/wp-content/uploads/2018/08/AFRTechnology.jpg)

There are [many different ways](https://towardsdatascience.com/face-detection-for-beginners-e58e8f21aad9) to accomplish this basic process of creating abstract models of the face.

And finally, we compare the measurements in the abstract model against measurements in a large database of candidate faces. You can do this quickly because you are working with a few dozen measures (distance between eyes, distance between edges of the mouth, distance between edge of mouth to eye, etc.). You would calculate the difference between the face you are trying to identify, and each face in the database by comparing the length of each line. If the total distance between all of the features falls below a threshold, then the faces are flagged as a match to be examined further by a human, or some action is triggered (unlocking your phone or your front door). 

![](https://www.researchgate.net/profile/Abdullah_Al-Murad/publication/326682312/figure/fig1/AS:653988944957442@1532934523611/Face-recognition-workflow.png)

Assuming that the photos are taken in good light with forward-facing subjects and decent resolution cameras, what do you anticipate being a challenge with this process? Are facial features static data points that never change? Or would our facial grid vary widely based upon expressions and angles?

![](https://www.mathworks.com/matlabcentral/mlc-downloads/downloads/submissions/45750/versions/1/screenshot.jpg)

Note that some features, like distance between the eyes and size of the nose, will be static. Others, like the edges of the mouth or the size of lips, will be highly dependent upon the expression. The models that match faces can weight certain features more than others to account for expressions in this way. 

Stated another way, some features convey more information that others. [This paper](https://www.sciencedirect.com/science/article/pii/S0010027718302397) explores which facial features, when changed, render the individual most unrecognizable and result in the biggest drop in correct matches to the database. This graphic from the paper gives you an intuitive sense of what the computer algorithm might experience as features are "corrupted" in the images. 

![](https://ars.els-cdn.com/content/image/1-s2.0-S0010027718302397-gr2_lrg.jpg)

So if you are trying to escape the country by crossing a border, which feature would you try to disguise? 

![](https://image1.masterfile.com/getImage/NjE5LTA1ODMyMzc0ZW4uMDAwMDAwMDA=AF4WWd/619-05832374en_Masterfile.jpg)

## Trees

![](https://cdn.theatlantic.com/assets/media/img/posts/2018/12/Boston_tree_diff/390d37b06.gif)

![](https://miro.medium.com/max/700/1*RqsTOuZbqbfH_yZCPCtcGQ.gif)

![](https://miro.medium.com/max/600/1*wIsDPFDS_B2wD1JeXB0k4A.gif)

https://medium.com/descarteslabs-team/descartes-labs-urban-trees-tree-canopy-mapping-3b6c85c5c9cc



https://cran.r-project.org/web/packages/ForestTools/vignettes/treetopAnalysis.html

![](/assets/img/lidar1.png)



## Buildings

![](https://static01.nyt.com/newsgraphics/2018/07/17/all-buildings-in-us/941536000c71273a13f8f5a891b1b2f1e316c136/tall-suburbs-mesa-800.jpg)

https://www.nytimes.com/interactive/2018/10/12/us/map-of-every-building-in-the-united-states.html




## Guess the Profession from the Image

https://towardsdatascience.com/train-image-recognition-ai-with-5-lines-of-code-8ed0bdd8d9ba

![](https://miro.medium.com/max/700/1*BZB3eUcXb6atYuxJ6npVeQ.jpeg)

![](https://miro.medium.com/max/420/1*kgFf3orScs_NwQyspLslAQ.jpeg)

For this tutorial, we have provided a dataset called IdenProf. IdenProf (Identifiable Professionals) is a dataset that contains 11,000 pictures of 10 different professionals that humans can see and recognize their jobs by their mode of dressing. The classes of professionals whose pictures are in this dataset are as below:

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

This dataset is split into 9000 (900 pictures for each profession) pictures to train the artificial intelligence model and 2000 (200 pictures for each profession) pictures to test the performance of the artificial intelligence model as it is training. IdenProf has been properly arranged and made ready for training your artificial intelligence model to recognize professionals by their mode of dressing. For reference purposes, if you are using your own image dataset, you must collect at least 500 pictures for each object or scene you want your artificial intelligence model to recognize.

## Assignment:

Define three features

https://www.wikihow.com/Tell-What-Someone-is-Like-from-Their-Handwriting
