## Resubmission
This is a resubmission. In this version I have:

* Imported used base packages that were not included in the NAMESPACE file

## Test environments
* MAC OS X 10, R 3.1.2
* Ubuntu 14.04, R 3.2.2
* Windows 10, R 3.2.2

## R CMD check results
There were no ERRORs or WARNINGs. 

There was 2 NOTE:

* checking CRAN incoming feasibility ... NOTE
  Maintainer: ‘Jacinto Arias <jacinto.arias@uclm.es>’
  New submission

  The submission comes actually from his maintainer

* checking R code for possible problems ... NOTE
  plotCumulativeRank: no visible binding for global variable ‘continuous’
  plotCumulativeRank: no visible binding for global variable ‘value’
  plotRankDistribution: no visible binding for global variable ‘method’
  plotRankDistribution: no visible binding for global variable ‘value’

  As this is using ggplot2, these variables correspond with the internal
  data.frame columns names that are incorporated into the call enviroment.

## Downstream dependencies
  We did not run checks on downstream dependencies, because there were no behaviour modifying changes to the code.