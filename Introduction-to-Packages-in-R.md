---
title: "Introduction to Packages in R"
author:    
    -  "RSN_Thinklabz_Chennai"

output:
  html_document:
    keep_md: true
    toc: yes
    
    

---








# Preamble
The one distinguishing feature which keeps R dynamic is the availability to create and upload Packages which can define various methods (i.e functions) on R objects. The packages created and uploaded by Eminent Scholars and Data Scientists can be downloaded, installed and utilised by any user all over the world. The main aim of a Package is to make user easily understand functions in it towards particular purpose.
   
   R packages are a collection of R functions, complied code and sample data. They are stored under a directory called "library" in the R environment. By default, R installs a set of packages during installation.  When we start the R console, only the default packages are available to us. Other packages which are already installed have to be loaded explicitly to be used by the R program that is going to use them.
   
   
## Get to know about Packages 
The following table gives the toolkit of functions which can be used to handle Packages in R
<table class="table table-striped" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>Packages handling</caption>
 <thead>
  <tr>
   <th style="text-align:left;"> Command </th>
   <th style="text-align:left;"> Usage </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> .libPaths() </td>
   <td style="text-align:left;"> Get library locations containing R packages </td>
  </tr>
  <tr>
   <td style="text-align:left;"> library() </td>
   <td style="text-align:left;"> Get the list of all the packages installed </td>
  </tr>
  <tr>
   <td style="text-align:left;"> search() </td>
   <td style="text-align:left;"> Get all packages currently loaded in the R environment </td>
  </tr>
  <tr>
   <td style="text-align:left;"> install.packages("Package Name") </td>
   <td style="text-align:left;"> Install package directly from CRAN </td>
  </tr>
  <tr>
   <td style="text-align:left;"> install.packages(file_name_with_path, repos = NULL, type = "source") </td>
   <td style="text-align:left;"> Install package manually </td>
  </tr>
  <tr>
   <td style="text-align:left;"> library("package Name") </td>
   <td style="text-align:left;"> Load Package to Library </td>
  </tr>
</tbody>
</table>

   
## Need for R Packages
Packages are integral objects which aid us perform various operations in R. There are situations where default packages does not have function defined for performing the task which we are interested in. For overcoming this we can either create a function or if it is available with any other package which is not in our system we can use the function after installing and loading the package.    

   One such example for this is skewness and kurtosis calculation in R, eventhough R is a statistical programming language default packages do not have function to compute the above measures, we can overcome this by making use of packages such as e1071, moments, SciencesPo etc  

# Some useful Packages 
   Having known the basics about packages in R, we shall look at some of the useful packages just to get an idea about how much they are utilised. For this let us consider some of the areas where additional packages are used   
   
   1) Loading and converting data
   2) Data wrangling
   3) String handling
   4) Date handling
   5) Pipe operator
   6) Data visualization 
   6) Application development

## Loading and converting data
For loading data from various sources we use package called **`foreign`**.      
foreign package is used for Reading data in following file formats.   

+ 'Epi Info'   
+ 'Minitab'   
+ 'S'   
+ 'SAS'   
+ 'SPSS'   
+ 'Stata'   
+ 'Systat'   
+ 'Weka'   
+ 'dBase'   
It can also be useful for writing data to above file formats

## Data wrangling
For data wrangling we use a package called **`dplyr`**    
dplyr is based on grammar of data manipulation, providing a consistent set of verbs that help us solve the most common data manipulation challenges such as:
   
   + Adding new variables that are functions of existing variables   
   + Selecting variables based on their names.   
   + Picks cases based on their values.   
   + Reduces multiple values down to a single summary.   
   + Changes the ordering of the rows.
   + Combining tables
   
## String handling 
Working with categorical data is very important task and **`stringr`** is one of the packages which helps us perform various operations on strings such as
   
   + Finding number of characters
   + Splitting a string to list(which then can be converted to vector)
   + Joining multiple strings and also values of variables with strings   
   + Finding existence of pattern 
   + Replacing pattern with another
   + Counting occurence of pattern
   + Trimming whitespaces in a string
   + Truncating a string to represent short form
   
## Date handling
**`lubridate`** is the package which we use for handling date and time objects in R 
   
   + Assignment of date time objects
   + Extracting parts of date time object
   + Sequence generation
   + Difference calculation
   + Time span measuring
   + Dealing with daylight saving
   
## Pipe operator
Pipe operator can be used in almost all operations in R. It enables us understand the action done easily and these are introduced by **`magrittr`** package. It simply gets the data in one side and provide it as input for function on the other side i.e we use x %>% f, rather than f(x). This package helps us do the following with ease
   
   + Evaluating nested functions
   + Evaluating and assigning the value back to the variable
   
## Data visualization
Data Visualization in most convenient way can be achieved through **`ggplot2`** and interactive plots can be obtained using **`plotly`**. These packages can be used to perform following operations
   
   + Customising Title and axes lable font styling
   + Changing background of plot
   + Scaling axes
   + Making plot interactive
   + Faceting plot
   
## Application development
We can create web apps using **`shiny`** and **`shinydashboard`** packages, the functions are easy to learn and we can perform following operations using these packages 
   
   + Creating a web app
   + Customize theme
   + Performing operations available with R and displaying them
   
# Final Note 
This notes has given some operations which can be performed using some non default packages.   
 The above packages are a small example of vast availability in R. These are also updated over time and new functions are introduced. Keep visiting blogs to get News about packages. Feel free to reach out for queries

    
