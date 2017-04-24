---
layout: post
title:  Brief on Lab
date:  2017-02-28
categories: [Summary] 
comments: true
---

#### Lab 4: Introduction to CrimeStat
Lab 4 introduced another University of Massachusetts creation: CrimeStat. This program analyze crime data, we used it to process Break and Enter (B&E) crime data, residential B & E commercial B & E and car theft, in Ottawa, Ontario. The purpose was to explore different tools to identify patterns in the data.

![First Map: Risk-Adjusted Nearest Neighbour Hierarchical Cluster of Crime in Ottawa. Second Map: 2006 Ottawa Crime Hot Spot Analysis]({{ site.url }}/img/HotSpot.jpg){: .pull-left}{:height="3000px" width="500px"}

First, Nearest neighbour analysis was performed to determine if the event for each crime were spatially autocorrelated. Then a Moran's I analysis were performed, to examine the events in relation to specific areas, in this lab we looked at dissemination areas (DA).  


The results were then processed in two tools, fuzzy mode analysis and nearest neighbor hierarchical clustering. 

Fuzzy mode method uses point-based analysis, to identify crime location and the crimes to it’s proximity, using the radius. The “Fuzzy” in fuzzy mode refers to the analysis showing areas where a number instances occur (small hot spot areas) rather than exact locations. Since all points within the user defined search areas are counted, points are counted multiple times. This could artificially skew results in small spatial area like downtowns. This could be that the “2006 Ottawa Crime Hotspot Analysis” map where high concentration is located downtown might not reflect the reality.

![Ottawa 2006 Residential Crime Density Interpolation]({{ site.url }}/img/Kernel Density.jpg){: .pull-right}{:height="3000px" width="500px"}

The nearest neighbour hierarchical spatial clustering technique calculates high crime areas and represents them by ellipse compared to points by Fuzzy mode analysis. The technique simulate confidence interval with a Monte Carlo simulation to find clustering of crime. The parameters controlling nearest neighbour selection process are chosen by the user. In this lab a minimum of 10 points  were established and a threshold distance of 500 meters was set, the result we see in the map attached “Risk-Adjusted Nearest Neighbour Hierarchical Spatial Cluster of Crime in Ottawa”. The “hierarchical” in nearest neighbour hierarchical spatial clustering refers to analysis which provides order of clusters, the points that unusually close together are clumped together at the first order. The first-order clusters are then tested for second order clustering, this is similar to the first-order clustering except that the cluster centers are now treated as “points” which themselves are clustered. This process continues to subsequent other, until there is no longer any clusters. In the map, we identified 3 orders of clustering. This analysis is different to the fuzzy mode technique as it provides users to manipulate the amount of points (crime instance) resulting in changeable visual catchment.    

The final step was to perform 
single and dual kernel density analysis on car theft in the Ottawa area. Single kernel density considered absolute density of crimes, while dual considered the population and crime, resulting in a relative density of crime.



***



#### Lab 3: Introduction to Geograpically Weighted Regression
The purpose of this lab was to explore the different uses and values of Ordinary Least Squares(OLS) regression  and Geographically Weighted Regression (GWR). Both methods demonstrate the strength of the relationship between two or more variables. OLS provides a global average, and GWR takes local geography into account.

We looked at the relationship between a child's social skills and a small set of variable related to the child (example: Physical abilities and language abilities, gender, ESL) and their neighbourhood (Census Enumeration Area: income). 

I looked at the relation between a child’s social skills and a small set of variables related to the child, such as if he or she is coming from a lone parent household, is a recent immigrant or visible minority, and their neighbours (Vancouver). My analysis found that there is a strong relationship between language skills, English as a Second language, and Income, especially in the East side of Vancouver. This could be a result of the socioeconomic makeup of Vancouver eastside. Immigrants who do not speak English as a first language tend to have lower paying jobs, which results in poorer language skill attainment in their children.

![Vancouver Children Language Skill in Relation to Income using Geographically Weighted Regression ]({{ site.url }}/img/languageskillandincome.jpg){: .pull-right}{:height="200px" width="1000px"}

Geographically weighted regression (GWR) emphasizes local analysis rather than global parameters. The focus on locality provides increased model accuracy and prediction power for specific study regions such as in the field of environmental justice. A study published in the Social Science Research journal by Angela Gilbert and Jayajit Chakraborty looked at potential health risks from exposure to hazardous air pollutants in Florida and its relationship with race/ethnicity and socioeconomic status. Their study, “Using geographically weighted regression for environmental justice analysis: Cumulative cancer risks from air toxics in Florida", addressed the gaps that traditional regression techniques failed to discern from spatial variation in statistical relationships. The researchers used geographically weighted regression to explore the spatial variability in analytical results and to determine the significance of statistical association between health risk and race/ethnicity or socioeconomic status. They used census tract level estimates of cumulative cancer risk from the EPA with Census 2000 data and GWR to determine that race and ethnicity are significantly related to cancer risk in Florida. They found that conventional regression such as OLS can hide local variation in statistical relationships relevant to environmental justice analysis (Gilbert and Chakraborty, 2010). 

![Vancouver Children Social Skill in Relation to Income and ESL using Geographically Weighted Regression ]({{ site.url }}/img/incomeandesl.jpg){: .pull-right}{:height="200px" width="1000px"}

Bibliography:

Gilbert, A., & Chakraborty, J. (2011). Using geographically weighted regression for environmental justice analysis: Cumulative cancer risks from air toxics in Florida. Social Science Research,40(1), 273-286. doi:10.1016/j.ssresearch.2010.08.006

#### Lab 2: Exploring Fragstats
This lab was an introduction to FragStats. FRAGSTATS is software from the University of Massachusetts.  We used data from Edmonton, Alberta between 1966 and 1976 to explore three metrics of FRAGSTATS, Class metric, Aggregation and Diversity. This data is Canada Land Use Monitoring Plan (CLUMP) data, which is a direct result of Canada’s development of GIS.

From the FRAGSTAT results, a transition matrix was created to show land use change from 1966 to 1976 in excel. We can observe that an increase in urban areas, at the lost of cropland/improved pasture and forage crops. This corresponds to the maps. That urban areas increase between 1966 to 1976, both outwards from the core as well as westward, southward and eastward. 

![Transition Matrix]({{ site.url }}/img/pivot.png){: .pull-right}{:height="200px" width="1000px"}

#### Lab 1: Spatial stats using Modelbuilder tutorial

According the Centers of Disease Control and Prevention, heart disease is the number one leading cause of death in the United States. In 2011 alone, 610,000 people died of heart disease, stroke and other cardiovascular diseases, claiming more lives than all forms of cancers combined. This week’s lab uses Centre for Disease Control data to map hot and cold spots of heart disease in the southern United States from 1999-2015. Attached is one of sixteen maps produced, showing the results for 2014. The findings showed that heart disease is concentrated more in rural areas compared to urban ones. This finding is supported by a study done in 2004 which looks at “The Importance of Place of Residence: Examining Health in Rural and Nonrural Areas” (Eberhardt and Pamuk, 2004), which identified that the prevalence of diabetes in rural areas and them having poorer health statuses lead to an increased risk of cardiovascular disease. Although urban environments are more likely to see larger disparities in socioeconomic status, higher violent crime rates, and higher prevalence of psychological stressors that accompany the increased density and diversity of cities, the analysis found that a higher concentration of cold spots of heart disease are found in and around urban areas such as Atlanta and Washington D.C. The findings support the basic understanding of heart disease is caused by many behavioural risk factors, such as tobacco use, unhealthy diets, obesity, physical inactivity, and harmful use of alcohol which rural areas are more vulnerable such activities. 

![Heart Disease Hot Spots and Cold Spots in 2014, by County in the Southern United states ]({{ site.url }}/img/Lab1Hotspot-01.jpg){: .pull-right}{:height="200px" width="1000px"}