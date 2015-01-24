---
title       : Course project Part 2, slidify
subtitle    : Evaluating your weight
author      : Bestco
job         : Student
framework   : io2012       # {io2012, html5slides, shower, dzslides, deck.js, dzslides, landslide, slidy ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap, shiny, interactive}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Background
The number of people that are over-weight or obese are increasing all over the world. This is troublesome because they are risk factors for a number of diseases such as diabetes, stroke and coronary heart disease.

---
## What is Body Mass Index (BMI)

1. BMI = Weight / Height^2
2. Weight in kilogram and height in meter
3. Used to evaluate whether one's weight is optimal.

---
## BMI calculation
For example, if you are 1.75 meter high and weight 75 kilogram, your BMI calculation and evaluation of your weight is as follows:

```r
height = 1.75
weight = 75
result <- function(height, weight) {
  bmi <- weight / height ^ 2
  if (bmi < 18.5) h <- "You are under-weight"
  else if (bmi <= 25) h <- " You have an optimal weight"
  else if (bmi <= 30) h <- "You are over-weight"
  else h <- "You are obese"
  h
}
result(height, weight)
```

```
## [1] " You have an optimal weight"
```

---
## Conclusion
BMI has been used frequently in evaluating one's weight. Doctors gave advices to their patients if they are over-weight or obese.
