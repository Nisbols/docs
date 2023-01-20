---
title:  "R Cookbook"
date:  2020-12-26  
summary:    
draft:  
---

- - - -
Code snippets 
- - - -
## Dice Game
```r
# set the roll function with two 6-sided dice as the default
roll <- function(die = 1:6, size = 2, prob = NULL) {
	dice <- sample(die, size, replace = TRUE, prob)
	sum(dice)
# example of probability; 1 - 5: 1/8; 6: 3/8
# c(1/8,1/8,1/8,1/8,1/8,3/8)
}
```