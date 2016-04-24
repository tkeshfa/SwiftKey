---
title       : Word Prediction Application
subtitle    : SwiftKey
author      : Sherif EL Farahaty  
job         : Data Scientist
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

### The goal is to build a next word prediction application in R using the data provided by SwiftKey Co.,



### In the next slide we will introduce the used approch that come up with such prediction also we will describe on how to use the application.

--- .class #id 

## Corpus Creation

1. Download of the data including Twitter , News & blogs
2. Extract sample which represents only 20% from the entire data. 
2. Cleaning of the data
    removing strange characters
    no stemming / removal of stop words etc. at this stage!
3. Creation of 2-gram , 3-gram and 4-gram combinations.
4. Creation of a key using stemmed lower case first / second word of n-grams
  enables for quick search based on user input
6. Combining the 3 documents / partial corpus into one

--- .class #id 

## Algorithm

1. The alogrithm relies on 4-grams with 3-gram fallback using a sinlge key of stemmed words. It means that it is fast and the corpus is small. That is important to keep when adding additional features.

2. The addition of a cache with previously used combinations of words would be a good addition for a next version.

--- .class #id 

## Interface / GUI

Following is the screen shoot from the application

<div style='text-align: center;'>
    <img height='400' width='800' src='screen.png' />
</div>

In order to access the App of Next Word Prediction [click here]

[click here]: <https://tkeshfa.shinyapps.io/Project_2/>

--- .class #id 

## Thank You
