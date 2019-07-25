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
