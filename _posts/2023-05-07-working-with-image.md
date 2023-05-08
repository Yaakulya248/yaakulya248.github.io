---
layout: post
title: Assignment 2
excerpt: "Image Analysis Assignment"
modified: 5/29/2023, 9:00:24
tags: [intro, beginner, image, tutorial]
comments: true
category: blog
---

# **A comparative analysis and classification of randomly generated cluster of photos using 'Orange'**
*Authors: Yaakulya Rabbani, Sami Areez*


An assignment where we fidget around with image analysis using a data mining and processing software Orange with randomly sorted images from four distinct categories. 

This is a two part assignment. In the first part, we collect an assortment of randomly gathered pictures belonging to a specific niche/category (which we call as ‘image class’) and see how we can actually distinguish and sub-categorize those images using image embedding algorithms provided by Orange followed by neatly laying those sub-categories into hierarchical clusters.

For the next part, we build upon the activities of the previous step and take it up a niche by incorporating similar banks of images but this time with an additional 3 different categories taking our number of image sources/classes into 4.
We then replay the same simulation as last time, and subsequently test out the prediction mechanism of Orange done on the basis of analysis of several features/data points of each of the images of the respective collections we gave it.

All the individual sources along with the combined collection of the photos used in the experiments are indexed at the end of the page.

## - Project Outline:

### About the images

The images for this entire experiment were taken from sources like WikiArt and Akaash image libraries (the links to each individual library have been cited at the end). The images sourced for each distinct category were picked at random from the first couple of webpages of each site to eliminate any chance of biases that might hinder the validity of the experiment outcomes.


### Tools used

Much like a corpus, analyzing an entire cluster of photos and segmenting them is something not possible by bare humane abilities. Orange aids that procedure by using image embedding and sorting algorithms accessed from its server remotely and analyzing over 2000 different data points(attributes) of each individual picture to put into contrast with the attributes to all the other photos. 

:# Part 1: Hierarchical clustering using Dendrograms:


*Segment Outline:*
 - Category: Romanesque Architecture
 - Number of photos in the sample: 37
 - The image collection used can be found here 


To start with, we first import our collection into the dataset and do a primary check for the metadata:

<figure>
<img src="/assets/orange/1.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

First we choose the entire folder of our images and *import* the photos as such. We can then access the collection in the application itself using the image viewer. The primary metadata of the images can be found using the *Data Table*.


The metadata we get: 
<figure>
<img src="/assets/orange/2.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>


We do get some ‘metadata’ but all we really get are the size dimensions and the names and origins files of the photos - something we can’t really use for anything at all.



*That’s where Image Embedding comes in*.

<figure>
<img src="/assets/orange/3.1.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

After running our dataset through image embedding we get a plethora of very useful pieces of information (metadata) that we can use for our next step


<figure>
<img src="/assets/orange/3.2.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

*The metadata we now get*:
<figure>
<img src="/assets/orange/4.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>



We can use any of the several embedding algorithms provided in the system software that suits our specific needs/types of photos in context. What we get are over 2000 individual characteristics/data points which the system picks up, examines and analyses to categorize each of the photos into various clusters and sub-clusters.








### Hierarchical Clustering: Dendrogram:


<figure>
<img src="/assets/orange/5.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

This is the final product we get after our processing up until this point. Based on the characteristics of all the photos (2048 individual data points), we get a hierarchical structure called Dendrograms which sort of looks like the root network of a tree. The concept is pretty straightforward and visually intuitive as all it does is sort it into categories and subcategories based on all the characteristics that we previously derived and processed in our procedure.


Let’s have a look at some excerpts from the graphs as examples to make sense of the entire thing:







### Example 1: Front Facing right angle

<figure>
<img src="/assets/orange/6.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>


As we can see, the clustering in this example is visually on point. Both the pictures have a VERY strong similarity in terms of image structure and the size and shape of the subjects concerned. It is basically photos of ancient fort-like structures with a seemingly 90* bank towards the camera/viewpoint as the foreground and the blue sky as the background.

All of the following examples also portray a randomly chosen pair of photos that have been clustered based on the amount of visual similarities and characteristics they possess. 

### Example 2: Lush Greeneries

<figure>
<img src="/assets/orange/7.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

Photos of remote forts and castles surrounded by a lush landscape of forests.

### Example 3: Curved Entrances and Alleyways 

<figure>
<img src="/assets/orange/8.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

An entire subcategory of photos that seem to share a common architectural philosophy in terms of interior designs. 

Every single one of the architectures, being distinct and mighty beautiful in their own rights, seem to share a structural design incorporating curved ceilings and entrances and long alleyways. Also interesting to note that ALL of the photos are of famous churches & chapels scattered across Europe, which does help explain a lot.

### Example 4: Pillar Art


<figure>
<img src="/assets/orange/9.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

Pillar art and carvings typically found in historical monuments and structures of Europe - a signature of medieval European architecture. And as expected the algorithm lists these together in the same branch of the dendrogram given their visual resemblance and congruent characteristics.


- ## Final Product:
*Image Grid after Image Embedding*

<figure>
<img src="/assets/orange/10.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

Our final cluster incorporating all of the clustering that we did & discussed up until now, neatly summed up in a grid arranged on the basis of similarities across the dataset.

### Workflow to get to this point:


<figure>
<img src="/assets/orange/11.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

### Course of Action:

1. Enter our entire set into the application using the ‘Import Images”
2. After having a look at the photos themselves and their primary metadata (dates, dimensions), we pipe it into the ‘Image Embedding’ function using a suitable algorithm.
3. After getting the attributes/image vectors to each of the 37 images of the set, we can analyze it view it
4. Set up the Hierarchical Clustering using Dendrogram for our final output
5. View the images as we did above.




:# Part 2: Classification, Predictions, and Anomalies:

*Working with 130+ images*


Now, we can take our learnings from our previous experiment and take it one step further.
We-
1. Work with 4 different categories of images consisting of of total of over 130 images
2. After repeating the same procedure as the previous part, we go ahead and set up a prediction model and see how the images fare in it.

### Segment Outline:
 - Names of Categories:
 1. Romanesque Architecture - 37
 2. A Gulf of Images (Architecture) - 37 
 3. Medieval Structures and Architectures (Negative: 17-19th Century) - 32 
 4. The Edge (Architecture) - 26

 - Link to the photo collection: [Same as the previous](https://drive.google.com/drive/folders/1zCOBYnXtL3mBae2knFCVnmiOmGEUi8ay)

**A snapshot of the entire collection of the photos used here:**

<figure>
<img src="/assets/orange/12.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>
     
## - Image Embedding:

We follow through the same course of actions that lead us to the table containing 2048 individual attributes/data points of all the images in our collection that we shall subsequently use for clustering and comparing.



<figure>
<img src="/assets/orange/13.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

## Hierarchical Clustering: 

### - Example 1:

<figure>
<img src="/assets/orange/14.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

### - Example 2:
 
<figure>
<img src="/assets/orange/15.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

This one in particular might be a bit off (as is the case for few values for any data analytics project) as the visual similarities or the congruent attributes of the images that made the system cluster them together might be immediately evident.

That being said and done, now we move on to the next and final step of our project, that is creating a prediction model (based on previously generated image attributes) using **Confusion Matrix**. 

After constructing the matrix, we can cross examine each of the samples itself and get an idea of the effectiveness of the model and the overall quality of our custom dataset itself.

### Confusion Matrix: 

 - Actual vs Predicted Values
 - Shows the number of instance of each combination

Confusion matrix is a pretty straightforward concept: a square matrix that is constructed with the actual results (classes of each image) on the horizontal axis and the predicted results - the class of the image as perceived by the algorithm on the basis of its characteristics - on the vertical axis.




<figure>
<img src="/assets/orange/16.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>






<figure>
<img src="/assets/orange/17.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>




### Interpretation:

 - The diagonal line lists all the results that were predicted correctly by the algorithm (Actual = Predicted); i.e - where the image concerned actually does belong to the class/category it bears resemblance to.
 - The ones aside from/around the diagonal are the ones where the actual and the predicted class of the images don’t match up: the image bears strong resemblance to a different category than the one it actually belongs to. The further the image from the diagonal (the more to the edge), the more resemblance it bears to the image category it was predicted to be by the algorithm than the one it actually belongs to.

**Prediction and Cross Validation: A Sample analysis**

<figure>
<img src="/assets/orange/18.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

As we can see from the sample, it’s one of the farthest away from the diagonal - right on the corner. WHich means the algorithm is strongly convinced that based upon the visual resemblance, the images follow the pattern and look visually similar to another category than they are to their own category.

And we can also see why: the way that the people are gazing over the horizon sitting at where it seems like the edge of a balcony/beach, this photo bears visual resemblance as if it belongs to the image category The Edge; whereas it was actually sourced from A Gulf of Images.

### Test and score results: 

<figure>
<img src="/assets/orange/19.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>


 - Area under the ROC curve (AUC) is really high 
 - The Classification Accuracy is very accurate. 
 
 
 
## Artitecture used for testing 130+ images: 


<figure>
<img src="/assets/orange/20.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

After repeating the same workflow we did in chapter 1, we pipe the photos into an image testing function for testing and sorting. In our case, we use the ‘Logistical Regression’ algorithm to model our analyze before piping it into our testing program where it is processed before finally sending it in to sort it in the Confusion Matrix

<figure>
<img src="/assets/orange/21.png" style="width:200%; height:200%;"/>
<figcaption style="text-align: center;">First steps: Importing our dataset</figcaption>
</figure>

This one a combination of both the segments of this assignment as we incorporate the hierarchical clustering as well (alongside the adjacent workflow leading up to the confusion matrix for comparison)

# Index:

 - Data Set #1 : Romanesque Architecture (37 Images)
 [Link](https://www.wikiart.org/en/paintings-by-genre/architecture?select=featured#!#filterName:featured,viewType:masonry)

 - Data Set #2 : A Gulf of Images (Architecture) (37 Images)
[Link](https://akkasah.org/en/results/?filter=collection_name%3EA%20Gulf%20of%20Images;;&queries=&pageid=undefined)

 - Data Set #3: Buildings and Architecture (Negative: 17-19th Century) (32 Images)
[Link](https://www.clevelandart.org/art/collection/search?i=3&search=Architecture)

 - Data Set #4: The Edge (Architecture) (26 Images)
[Link](https://akkasah.org/en/results/?filter=collection_name%3EThe%20Edge;;&queries=&pageid=undefined)

Link for the above images data: [Drive](https://drive.google.com/drive/folders/1zCOBYnXtL3mBae2knFCVnmiOmGEUi8ay)

