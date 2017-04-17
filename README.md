This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

Grant D. Jacobsen and Matthew J. Kotchen evaluate in their paper "ARE BUILDING CODES EFFECTIVE AT SAVING ENERGY? EVIDENCE FROM RESIDENTIAL BILLING DATA IN FLORIDA" (2013) the actual effects of building codes on residential energy consumption. Their main finding is that a tightening of the building energy code in the year 2002 is associated with a 4 percent and 6 percent reduction in electricity and natural gas consumption of residences in Gainesville, respectively.  
In this problem set you will reproduce the main findings, practice in R programming and learn about some econometric methods.

You can download the article from the following page: http://www.mitpressjournals.org/doi/abs/10.1162/REST_a_00243#.WO3sjvnyjIU.

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
if (!require(devtools))
  install.packages("devtools")
source_gist("gist.github.com/skranz/fad6062e5462c9d0efe4")
install.rtutor(update.github=TRUE)

devtools::install_github("LEilts/RTutorBuildingCodes", upgrade_dependencies=FALSE)
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorBuildingCodes)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorBuildingCodes")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorBuildingCodes",
       load.sav=TRUE, sample.solution=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
