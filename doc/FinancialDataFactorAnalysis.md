<link rel="stylesheet" href="http://netdna.bootstrapcdn.com/bootstrap/3.0.3/css/bootstrap.min.css">
<style type="text/css"> body {padding: 10px 30px 10px 30px;} table,th, td {text-align: center;} </style>


Boats Segmentation: Factor Analysis
========================================================

**Team names**

#Temp comment to fix Knit HTML issue:
#library(knitr)
#knit2html("/Users/ArinaB/Documents/Arina MBA/INSEAD-16D/P3/Big Data Analytics/AnalyticsProject/doc/FinancialDataFactorAnalysis.Rmd")

Business Decisions
---------------------------------------------------------
your text...


The Data
--------------------------------------------------------------


your text...


```
## Error in is.data.frame(frame): object 'ProjectDataFactor' not found
```

```
## Error in is.data.frame(frame): object 'ProjectData' not found
```

This is how the first 'r  min(max_data_report, nrow(ProjectData))' data looks:
<br>

<div class="row">
<div class="col-md-6">

```
## Error in data.frame(round(ProjectDataFactor, 2)): object 'ProjectDataFactor' not found
```

```
## Error in eval(expr, envir, enclos): object 'show_data' not found
```

```
## Error in rownames(show_data): object 'show_data' not found
```

```
## Error in cbind(row, show_data): object 'show_data' not found
```

```
## Error in is.data.frame(x): object 'dfnew' not found
```

```
## Error in change[1] <- "Variables": object 'change' not found
```

```
## Error in eval(expr, envir, enclos): object 'change' not found
```

```
## Error in eval(expr, envir, enclos): could not find function "gvisTable"
```

```
## Error in print(m1, "chart"): object 'm1' not found
```
</div>
</div>
<br> <br>

Our Approach
---------------------------------------------------

#### Factor Analysis in 6 steps

1. Confirm the data in metric 

2. Decide whether to scale or standardize the data

3. Check the correlation matrix to see if Factor Analysis makes sense

4. Develop a scree plot and decide on the number of factors to be derived

5. Interpret the factors (consider factor rotations - technical but useful)

6. Save factor scores for subsequent analyses

Let's follow these steps.


The data we use here have the following descriptive statistics: 

<div class="row">
<div class="col-md-6">

```
Error in data.frame(round(my_summary(ProjectDataFactor), 2)): could not find function "my_summary"
```

```
Error in rownames(show_data): object 'show_data' not found
```

```
Error in cbind(row, show_data): object 'show_data' not found
```

```
Error in is.data.frame(x): object 'dfnew' not found
```

```
Error in change[1] <- "Variables": object 'change' not found
```

```
Error in eval(expr, envir, enclos): object 'change' not found
```

```
Error in eval(expr, envir, enclos): could not find function "gvisTable"
```

```
Error in print(m1, "chart"): object 'm1' not found
```
</div>
</div>

#### Step 2: Decide whether to scale or standardize the data


your text...


```r
ProjectDatafactor_scaled=apply(ProjectDataFactor,2, function(r) {if (sd(r)!=0||is.na(r)==FALSE) res=(r-mean(r))/sd(r) else res=0*r; res})
```

```
## Error in apply(ProjectDataFactor, 2, function(r) {: object 'ProjectDataFactor' not found
```

Notice now the summary statistics of the scaled dataset:

<br>


<div class="row">
<div class="col-md-6">

```
Error in data.frame(round(my_summary(ProjectDatafactor_scaled), 2)): could not find function "my_summary"
```

```
Error in rownames(show_data): object 'show_data' not found
```

```
Error in cbind(row, show_data): object 'show_data' not found
```

```
Error in is.data.frame(x): object 'dfnew' not found
```

```
Error in change[1] <- "Variables": object 'change' not found
```

```
Error in eval(expr, envir, enclos): object 'change' not found
```

```
Error in eval(expr, envir, enclos): could not find function "gvisTable"
```

```
Error in print(m1, "chart"): object 'm1' not found
```



















