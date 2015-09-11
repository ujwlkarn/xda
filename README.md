# xda
R package for exploratory data analysis
---------------------------------------

This package contains several functions to perform initial analysis on any dataframe. 

- `numSummary(mydata)` function automatically detects all numeric columns in the dataframe `mydata` and provides their summary statistics 
- `charSummary(mydata)` function automatically detects all character columns in the dataframe `mydata` and provides their summary statistics 
- `Plot(mydata, dep.var)` plots all independent variables in the dataframe `mydata` against the dependant variable specified by the `dep.var` parameter 
- `removeSpecial(mydata, vec)` replaces all special characters (specified by vector `vec`) in the dataframe `mydata` with `NA` 
- `bivariate(mydata, dep.var, indep.var)` performs bivariate analysis between dependent variable `dep.var` and independent variable `indep.var` in the dataframe `mydata`

More functions to be added soon.

Installation
------------
To install the `xda` package, `devtools` package needs to be installed first. To install `devtools`, please follow instructions [here](https://github.com/hadley/devtools).

Then, use the following commands to install `xda`:

```s
library(devtools)
install_github("ujjwalkarn/xda")
```

Usage
-----
```s
library(xda)

#to view a comprehensive summary for all numeric columns in the iris dataset
numSummary(iris)

#to view a comprehensive summary for all character columns in the iris dataset
charSummary(iris)

# to plot all other variables against the 'Species' variable in the iris dataset
Plot(iris,'Species')
```
Please refer to the documentation of each function to understand how to use it. 
For example, to see the documenation for the `numSummary()` function, use `?numSummary`.

