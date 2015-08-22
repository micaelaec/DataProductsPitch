---
title       : Data Product Pitch
subtitle    : Changing the Way You Visualize the States Dataset
author      : Written by Micaela
framework   : io2012      # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow     # 
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
    
---  


<style> .title-slide {
       background-color: #6C2DC7; 
           } </style>
           
<style> .title-slide hgroup > h1, 
.title-slide hgroup > h2 {
  color: #000000;  /* ; #EF5150*/
} </style>

<!-- Limit image width and height -->
<style type='text/css'>
img {
    max-height: 500px;
    max-width: 964px;
}
</style>

<!-- Center image on slide -->
<script src="http://ajax.aspnetcdn.com/ajax/jQuery/jquery-1.7.min.js"></script>
<script type='text/javascript'>
$(function() {
    $("p:has(img)").addClass('centered');
});
</script>



## Problem

- You find a new dataset and are excited to see what is inside
- Where to start?
- Which is most interesting?
- How can I quickly and easily see bivariate relations between the variables?

--- 

## Example

The states dataset in R contains data from the 1970s on all 50 United States (first 10 rows shown below).  I would like to visualize the different relations amongst these variables.   
<!-- html table generated in R 3.1.1 by xtable 1.7-4 package -->
<!-- Sat Aug 22 00:41:54 2015 -->
<table border=1>
<tr> <th>  </th> <th> Population </th> <th> Income </th> <th> Illiteracy </th> <th> Life Exp </th> <th> Murder </th> <th> HS Grad </th> <th> Frost </th> <th> Area </th>  </tr>
  <tr> <td align="right"> Alabama </td> <td align="right"> 3615.00 </td> <td align="right"> 3624.00 </td> <td align="right"> 2.10 </td> <td align="right"> 69.05 </td> <td align="right"> 15.10 </td> <td align="right"> 41.30 </td> <td align="right"> 20.00 </td> <td align="right"> 50708.00 </td> </tr>
  <tr> <td align="right"> Alaska </td> <td align="right"> 365.00 </td> <td align="right"> 6315.00 </td> <td align="right"> 1.50 </td> <td align="right"> 69.31 </td> <td align="right"> 11.30 </td> <td align="right"> 66.70 </td> <td align="right"> 152.00 </td> <td align="right"> 566432.00 </td> </tr>
  <tr> <td align="right"> Arizona </td> <td align="right"> 2212.00 </td> <td align="right"> 4530.00 </td> <td align="right"> 1.80 </td> <td align="right"> 70.55 </td> <td align="right"> 7.80 </td> <td align="right"> 58.10 </td> <td align="right"> 15.00 </td> <td align="right"> 113417.00 </td> </tr>
  <tr> <td align="right"> Arkansas </td> <td align="right"> 2110.00 </td> <td align="right"> 3378.00 </td> <td align="right"> 1.90 </td> <td align="right"> 70.66 </td> <td align="right"> 10.10 </td> <td align="right"> 39.90 </td> <td align="right"> 65.00 </td> <td align="right"> 51945.00 </td> </tr>
  <tr> <td align="right"> California </td> <td align="right"> 21198.00 </td> <td align="right"> 5114.00 </td> <td align="right"> 1.10 </td> <td align="right"> 71.71 </td> <td align="right"> 10.30 </td> <td align="right"> 62.60 </td> <td align="right"> 20.00 </td> <td align="right"> 156361.00 </td> </tr>
  <tr> <td align="right"> Colorado </td> <td align="right"> 2541.00 </td> <td align="right"> 4884.00 </td> <td align="right"> 0.70 </td> <td align="right"> 72.06 </td> <td align="right"> 6.80 </td> <td align="right"> 63.90 </td> <td align="right"> 166.00 </td> <td align="right"> 103766.00 </td> </tr>
  <tr> <td align="right"> Connecticut </td> <td align="right"> 3100.00 </td> <td align="right"> 5348.00 </td> <td align="right"> 1.10 </td> <td align="right"> 72.48 </td> <td align="right"> 3.10 </td> <td align="right"> 56.00 </td> <td align="right"> 139.00 </td> <td align="right"> 4862.00 </td> </tr>
  <tr> <td align="right"> Delaware </td> <td align="right"> 579.00 </td> <td align="right"> 4809.00 </td> <td align="right"> 0.90 </td> <td align="right"> 70.06 </td> <td align="right"> 6.20 </td> <td align="right"> 54.60 </td> <td align="right"> 103.00 </td> <td align="right"> 1982.00 </td> </tr>
  <tr> <td align="right"> Florida </td> <td align="right"> 8277.00 </td> <td align="right"> 4815.00 </td> <td align="right"> 1.30 </td> <td align="right"> 70.66 </td> <td align="right"> 10.70 </td> <td align="right"> 52.60 </td> <td align="right"> 11.00 </td> <td align="right"> 54090.00 </td> </tr>
  <tr> <td align="right"> Georgia </td> <td align="right"> 4931.00 </td> <td align="right"> 4091.00 </td> <td align="right"> 2.00 </td> <td align="right"> 68.54 </td> <td align="right"> 13.90 </td> <td align="right"> 40.60 </td> <td align="right"> 60.00 </td> <td align="right"> 58073.00 </td> </tr>
   </table>

--- 


## Solution
With the Shiny app "Visualizing States Dataset," it is easy to select two variables from the states dataset and instantly see their bivariate relation.  In addition, the names of the states are given as points, allowing you to quickly see where each state falls in the correlation.

!['Pic1'](assets/img/ScreenShot1.png)

---


## Conclusion
"Visualizing States Dataset" is a useful data product that can be customized for any dataset you find yourself wanting to explore.

- By easily viewing the bivariate relations amongst the dataset's variables, you can make a plan for additional analyses.
- You might also see surprising and interesting results just in the scatterplots.  
  - On the previous page, for example, you might have been shocked by the strong positive relation between illiteracy and murder rate.



