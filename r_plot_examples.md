# r_plotting_samples
some plotting samples in sub plots
---
title: "R Plotting Samples"
output: html_notebook
---


## R Sample of Plots in Sub Plot

Using different mathematic functions as example of plotting in R.

```{r}
# Scope: Plotting a set of Graphs as example
par(mfrow=c(3,2))                       # number of sub plots
# Now the next 6 pictures will be placed on these 6 regions. :-)
# Plot 1 and parameters: Density
plot(density(runif(10)), lwd=2)
text(x=0, y=0.2, "10 units")        # Showing you how to place text at will
abline(h=0, v=0)
x=seq(0.01,1,0.01)
par(col="blue")                         # default colour to blue.
# Plot 2 and parameters: Sin & Cos
plot(x, sin(x), type="l", lwd=2)
lines(x, cos(x), type="l", col="green", lwd=2)
# Plot 6 and paramters: Sin
plot(x, sin(x*x), type="l")
lines(x, sin(2/x), col="orange")
# Plot 4 and paramters: Tan
plot(x, tan(x), type="l", lwd=3, col="orange")
# Plot 5 and paramters: lines
plot(x, exp(-x), lwd=2)
lines(x, exp(x), col="yellow", lwd=2)
# Plot 3 and paramters
plot(x, exp(x), type="l", col="green")
lines(x, log(x), type="l", col="orange")
```

![r_plotting6](https://user-images.githubusercontent.com/96922284/149657713-abeaa7cb-27d7-434d-9b2b-2404231ba59f.PNG)
