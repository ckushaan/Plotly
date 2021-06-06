# Peer-graded Assignment: R Markdown Presentation & Plotly

## Instructions

Create a web page presentation using R Markdown that features a plot created with Plotly. Host your webpage on either GitHub Pages, RPubs, or NeoCities. Your webpage must contain the date that you created the document, and it must contain a plot created with Plotly. We would love to see you show off your creativity! 

## Review criteria
- Does the web page feature a date and is this date less than two months before the date that you're grading this assignment?Bulleted
- Is the web page a presentation and does it feature an interactive plot that appears to have been created with Plotly?

## Submission

Click the following link for the presentation

**[Link](url)**

## Source Code

```
title: "R Markdown & Plotly"
author: "Kushan Sarathchandra"
date: "Published on `r format(Sys.time(), '%c')`"
output: ioslides_presentation
---

{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE, cache = TRUE, echo = FALSE, message = FALSE, warning = FALSE)


## Presentation Overview - `r format(Sys.time(), '%d %b %Y')`

I have created an interactive scatter plot using the plotly and mtcars dataset in R.

## Motorcars

{r cars}
library(plotly)
data("mtcars")
plot_ly(data=mtcars,x=~hp,y=~mpg,color = ~factor(cyl),
size=~wt,type="scatter",mode="markers")
```
