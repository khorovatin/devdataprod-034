---
title       : Canadian Ice Thickness Program
subtitle    : Explore Historical Canadian Ice Thickness Data
author      : Ken H.
job         : Developing Data Products Student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

This presentation was prepared in partial fulfillement of the course 
requirements of the Johns Hopkins Data Science Specialization course titled 
"Developing Data Products", as presented on Coursera by Brian Caffo, PhD, Jeff 
Leek, PhD, and Roger D. Peng, PhD.

We hear news stories on the results of scientific studies of Earth's climate 
almost every day. I feel that it is important to look at the data in order to 
better understand it and the conclusions drawn from those data.

The accompanying application allows you to look at one small set of climate 
data, graph it for selected data collection stations and time periods, and form 
your own conclusions about what is happening with our global climate.

This presentation and accompanying application has not been produced in 
affiliation with or with the endorsement of the Government of Canada.

--- .class #id 

## The Ice Thickness Program

The ice thickness data used in the accompanying application was gathered over 
a 68-year period starting in 1947. During the years 1947-2002 data 
was gathered from up to 195 stations throughout Canada, ranging from the high 
arctic to the St. Lawrence river. 

Starting in 2002 the data collection was stopped at most of the stations, so 
from that period forward only 11 stations continued reporting ice thickness 
measurements.

You can read more about the Ice Thickness Program at the Environment Canada 
[Ice Thickness Data](http://www.ec.gc.ca/glaces-ice/?lang=En&n=E1B3129D-1) 
web page.

--- .class #id 

## The Data

A summary of the imported and cleaned data:

```
## Error in `[.data.frame`(.data, , vars, drop = FALSE, with = FALSE): unused argument (with = FALSE)
```

```r
summary(allstndata)
```

```
##        ID            Name                Date                 Ice        
##  WEU    : 2056   Length:53851       Min.   :1947-09-22   Min.   :  0.00  
##  YRB    : 1836   Class :character   1st Qu.:1971-01-22   1st Qu.: 47.00  
##  YCB    : 1726   Mode  :character   Median :1979-05-04   Median : 81.00  
##  YLT    : 1695                      Mean   :1980-01-15   Mean   : 94.78  
##  YBK    : 1630                      3rd Qu.:1988-03-02   3rd Qu.:138.00  
##  LT1    : 1578                      Max.   :2014-06-13   Max.   :345.00  
##  (Other):43330                                           NA's   :72      
##    JoinName        
##  Length:53851      
##  Class :character  
##  Mode  :character  
##                    
##                    
##                    
## 
```

--- .class #id 

## Try It!

The accompanying "Shiny" web app for exploring the Canadian Ice Thickness 
Program data set can be found at the following address:

* https://kenh.shinyapps.io/Canadian_Ice_Thickness_Program

Source code for the web application can be viewed on GitHub at:

* https://github.com/khorovatin/devdataprod-033.

Source code for this presentation can be viewed on GitHub at:

* https://github.com/khorovatin/devdataprod-034.

*Enjoy!*
