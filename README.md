# R INTRODUCTION

# Creating a data set:

R works with packages that contain the techniques and functions you need. To start with some basic examples you need to know how to install and load a package. 

~~~~
## installing a package (i.e. alr4 - Applied Linear Regression 4th Edition Data Sets)
install.packages("alr4")

## loading a package
library(alr4)
~~~~

R data is manipulated with dataframes; data should be preferable in "matrix" form. You can create a data set, read a csv file or use a dataset already available (for example, doing a query from bigfoot - explained in "bigfoot-tutorials/rstudio/impala-test.R")

~~~
## create a data set: create variables using the c function. This function keeps values together.
x1 <- c("big","data","analytics")
x2 <- c(4, 5, 2)

## dataframe function - you can add a name to each variable
data <- data.frame(words=x1,count=x2)

data
      words count
1       big     4
2      data     5
3 analytics     2

## read a csv file - if the first row of the data is name for each variable, header should equal to TRUE
csv_data <- read.csv(name_of_file.csv,header=TRUE)
~~~

# Reviewing a data set:

You can review the structure of the data set using the following functions.

~~~~
## using a data set example from the alr4 package



