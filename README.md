# WebScraping
%%%% The packages need to be loaded at the beginning:
library(plyr)
library(dplyr)
library(reshape2)
library(xml2)
library(rvest)
library(stringr)
library(curl)
library(xtable)
library(ggvis)
library(knitr)
options(digits = 4)

%%%% phantomjs.exe must be saved in the working directories

%%%% The operation order of the scripts:
1. Function_ExtractLinks
2. ExtractAllHomeLinks
3. FinalExtractionAndSave
4. SaveHtmlPages


%%%% Functions of each scripts:
1. Function_ExtractLinks:
#Function ExtractLinks is used to extract all the home links from one searching-result page
#the input should be the link of a searching-result page
#This needs to be run before ExtractAllHomeLinks

2. ExtractAllHomeLinks:
#Extract All the Home Links
#Extract home links according to home type mainly

3. FinalExtractionAndSave
#This is to extract 22 fields of home information, and save the result into csv and txt files.

4. SaveHtmlPages
#After fetching all the home links, running this script to save all the home HTML pages.
