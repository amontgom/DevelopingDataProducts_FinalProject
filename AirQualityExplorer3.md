Air Quality Explorer
========================================================
author: Aaron Taylor
date: September 27, 2017
autosize: true

***
![title](data.jpg)

The Air Quality Explorer
========================================================

A simple Shiny App that lets you compare the different data of the airquality dataset. It can:

- Choose an arbitrary sample size (up to the size of the data)
- Compare any variables on the x- or y-axis
- Adjust the color by any variable
- Adjust the size by any variable
- Create a linear regression line
- create a smooth line, with 95% confidence interval
- Split the plot by rows according to a given variable
- Split the plot by columns according to a given variable

All of which lets you perform data analysis on airquality to your heart's content.

<div align="center">
<img src="smog.jpg" width=548 height=308>
</div>


The airquality dataset
========================================================


```r
dim(airquality)
```

```
[1] 153   6
```

```r
str(airquality)
```

```
'data.frame':	153 obs. of  6 variables:
 $ Ozone  : int  41 36 12 18 NA 28 23 19 8 NA ...
 $ Solar.R: int  190 118 149 313 NA NA 299 99 19 194 ...
 $ Wind   : num  7.4 8 12.6 11.5 14.3 14.9 8.6 13.8 20.1 8.6 ...
 $ Temp   : int  67 72 74 62 56 66 65 59 61 69 ...
 $ Month  : int  5 5 5 5 5 5 5 5 5 5 ...
 $ Day    : int  1 2 3 4 5 6 7 8 9 10 ...
```

```r
head(airquality)
```

```
  Ozone Solar.R Wind Temp Month Day
1    41     190  7.4   67     5   1
2    36     118  8.0   72     5   2
3    12     149 12.6   74     5   3
4    18     313 11.5   62     5   4
5    NA      NA 14.3   56     5   5
6    28      NA 14.9   66     5   6
```

Slide With Plot
========================================================

![plot of chunk unnamed-chunk-2](AirQualityExplorer3-figure/unnamed-chunk-2-1.png)
