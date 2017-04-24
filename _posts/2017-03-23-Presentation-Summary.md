---
layout: post
title: Presentation Summary
date: 2017-03-21
categories: [Presentation Summary]
comment: true
pinned: true 
---

****

## Assignment 1: Landscape Ecology and GIS

#### Distribution of invasive plants in urban environments is strongly spatially structured 

#### by Kateřina Štajerova, Petr Šmilauer, Josef Brůna, Petr Pyšek

Urban environment foster a wide range of habitats that harbour a great diversity of plant species, many of which are alien in origin. This study looks at how availabilty of different ecosystem types within a city area, as well as several parameters describing urban structure interact in determining the cover and identity of invasive alien species. 

##### Methods
Three parameters were set: 
- The presence/absence of ten habitat categories in 200 cells
- The abundance of each invasive neophyte, expressed in m2
- Whether the species was cultivated (yes or no)

Each cell "unit" was 200m x 200m 

 Predictors were established by length of roads, length of water courses, built-up areas, sealed surfaces, agricultural land, railways, and urban greenways. The proportion for each cell was computed using the ArcGis Pro Summarize Within tool. This statistics tool overlays a polygon layer with another to summarize the number of points, length of the lines, or area of the polygons within each polygon, then calculates attribute field statistics about those features within the polygons, or unit cells in this study. 

#### Results
 The study found that the transformation of ecosystem types were almost independent. There was a large amount of variation explained by the spatial predictors, but none shared with any measured variables. This suggested that some of the most important part of the identity and cover of present neophytes were missed. Alternatively, significant predictors might be events, structures or patterns that no longer exist. These study results suggest that the spatial structure and habitat quality of urban landscapes need to be taken into account for an effective management regime against the invasion of alien plants in the urban environment. 

### Other Presentation

#### A GIS approach to prioritizing habitat for restoration using neotropical migrant songbird criteria.

##### Holzmueller EJ1, Gaskins MD, Mangun JC.

Presented by: Paul Schwandt
I found this report and subsequent presentation thought provoking. That different areas respond to restoration effects differently. That reforesting a smaller high-priority area has a greater effect than reforesting a large low-priority area. This project demonstrated how GIS can be a tool for better land management. 

****

## Assignment 2: Health Geography and GIS 

#### Predicting the Risk of Lyme Disease: Habitat Suitability for **Ixodes scapularis** in the North Central United States 

###### by Marta Guerra,  Edward Walker, Carl Jones, Susan Paskewitz, M. Roberto Cortinas, Ashley Stancil, Louisa Beck, Matthew Bobo, and Uriel Kitron

Lyme disease is one of the most common vectorborne diseases in the United States. It is caused by the spirochete Borrelia burgdorferi and transmitted by *Ixodes scapularis*, also known as the blacklegged tick. In the Midwest, the distribution of Lyme disease is largely determined by I. scapularis. This species was first detected in Wisconsin in the late 1960s. The population expanded eastwards and southwards, remaining in relatively isolated populations. The white-tailed deer (*Odocoileus virginanus*) and white-footed mice (*Peromyscus leucopus*) serve as hosts for I. scapularis. However, it appears that the host population density is not what limits tick population, but rather the physical environment .

##### Site Selection:
Wisconsin: 28/59 state parks and forest were surveyed and selected

Michigan: three sites in Menominee , where ticks had been previously identified 

Illinois: sites in Ogle and Rock Island counties, sites along the Illinois River. 

##### Tick Collection 
The two dragging methods were used to tick in 138 sites in 1997: July, September- October and 1998: June and May. Along side obtaining samples from small mammals 

![Geographic distribution of Study sites]({{ site.url }}/img/Geographic distribution of Study sites.jpg){: .pull-left}{:height="1500px" width="300px"}

##### Sites the  were rated with data collected from the amount of ticks. 
* Negative (0) if I. scapularis  was never found on vegetation or small mammals host. 
* (1) if one stage of the tick was found, regardless of quantity. 
* (2) low density
* (3) high density 

##### Soil Date
Removal the layer of leaf litter, soil sample was collected
6 inches of topsoil
pH and the percentage of sand, silt and clay were measured for each sample = resulting in soil texture class

##### Forest Moisture Index
5 categories: dry, dry/mesic, mesic, wet/mesic, and wet 
Established through 50-m2  grid sample of each site 
Data Sources: 
Scaled at 1:40,000 from Landsat Thematic Mapper (TM) band 3 (red), 4 (near-infrared), 5 (mid-infrared)  and NDVI for hierarchies classification system into wetlands, urban areas, and upland areas. 

##### Landcover, elevation, and quaternary geologic data Illinois and Wisconsin and Michigan: 1:1,000,000 

![Predictive risk map of habitat suitability for *Ixodes scapularis* in Wisconsin and Illinois]({{ site.url }}/img/lymeriskmap.jpg){: .pull-right}{:height="1500px" width="300px"}

##### For Statistical Analysis: 
1.	Univariate analysis was initially performed by using chi square contingency tables to determine significant associations between site positivity and environmental variables coded as previously described. 
2.	Discriminant analysis was performed by using only the significant (p<0.25) environmental variables from the univariate analysis (41). 
3.	Tick presence was positively associated with deciduous dry/mesic and dry forests, fertile soils such as alfisols, sand and loamy/sand soil texture, and sedimentary bedrock. 
4.	There was a negative association with grasslands and conifer forests wet and wet/mesic forests. acidic soils such as spodosols, clay soil texture, and Precambrian bedrock. Elevation was not an important discriminator in the model
5.	Then a logistic regression analysis performed, its results were in agreement with the discriminant analysis model in the positive versus negative group as seen. The same variables were significant (p<0.05), and the model correctly classified 83.9% of the sites. 

##### Results
A predictive risk map generated from the logistic regression model, sites in Illinois along rivers and farther south showed high habitat suitability (60%-100%) and Wisconsin moderate suitability (26%-40%) are located in the western half of the state. Patchy areas of higher probability (60%-100%) are found in the central and northern portion. In Michigan, where only a small area of the Upper Peninsula was sampled, all sites had very dense tick populations, except for a site that was classified as excessively drained (>99% sand). 

##### In conclusion,
 This model can be used to help determine the risk of acquiring Lyme disease and other diseases transmitted by *Ixodes scapularis* by predicting which locations may be currently infested with the tick. Show suitable areas where new population could establish.

### Other Presentation

##### Landscape Elements and Hantaan Virus–related Hemorrhagic Fever with Renal Syndrome, People’s Republic of China

##### Yan L1, Fang LQ, Huang HG, Zhang LQ, Feng D, Zhao WJ, Zhang WY, Li XW, Cao WC
Presented by: Emily Grayston
Similar to the report I presented, this study analyzes environmental aspect to observe likelihood of a disease. This project uses multivariate logistic regression analysis of landscape elements such as elevation, NDVI, precipitation  annual cumulative air temperature, land surface temperature, soil type, and land use  to determine likelihood of Hemorrhagic fever with renal syndrome (HFRS). 

****

## Assignment 3: Crime analysis and GIS 

##### A GIS-based spatiotemporal analysis of violent trauma hotspots in Vancouver, Canada: identification, contextualisation and intervention

#### by Walker, B. B., Schuurman, N., & Hameed, S. M. (2014.)

The study used geographic information systems to plot 575 violent trauma incidents collected from the BC Trauma Registry, comprising the location, date, time and cause of every injury between 2001 and 2008. Due to data collecting protocols, confidentiality, regulations, and to eliminate minor incidents, only injury severity scores greater than 15 were used. This meant injuries to multiple body part were included and sports or self-inflicted injuries were excluded. The data was then classified into seven injury mechanisms: gunshot wound,  sharp object trauma, blunt object trauma, bodily force (ex: punch), and other assaults. This resulted in 575 incidents, which were mapped in space and time. Pearson’s Chi-squared test was used to determine the independence of variables against day/night, and the data was graphed in relation to time of day, day-night contrast, time of year and day of the week. These relationships were mapped in order to identify multivariate clusters. Using GIS, kernels density estimation was used to produce hotspot maps. Natural break (Jenk’s algorithm) was used to identify high concentration and the cut-off was manually adjusted to obscure several cases’ locations. To protect patient confidentiality, the kernel density bandwidth parameters and spatial scan window size were withheld to prevent reverse calculations. Finally, for the purpose of exploring the relationship between violent injury hotspots and socioeconomic deprivation, the researchers used the Vancouver Area Neighbourhood Deprivation Index (VANDIX) to calculate and classify quintiles and violent injury locations. 

Walker, Schuurman & Hameed found that out of the 575 violent trauma incidents reported, 518 were male victims and 57 female. This disparity corresponds with the findings in the literature, however the researchers do acknowledge the under-reporting of domestic violence. In addition, they found that violent trauma hotspots were most prevalent in Vancouver’s nightclub districts on Friday and Saturday nights. Researchers also found that there were higher rates of  violent trauma in the most socioeconomically deprived neighbourhoods, such as the Downtown Eastside. The analysis revealed that that different genders were victimized in different areas: Chinatown had only female victims,  Commercial Drive and stadiums featured only male victims. The researchers using VANDIX found that 77% of all severe violent injuries occurred within neighbourhoods in the two most deprived quintiles. However, club districts and Metrotown were notable exceptions. In night club districts, the high rate night-time incidents were related to alcohol-serving establishments. Metrotown was most likely due to the build urban environment. 

This study shows the value of using GIS in trauma epidemiology studies. It shows using both space and time to provide a more granular resolution picture of risk, highlighting that neighbourhood characteristics are used to describe context-specific urban violent spaces in a high-income country. Some of the limitations that researchers pointed out are that data recording procedures and confidentiality regulations limit the study to only severe trauma, “excluding cases where patients expired prior to arrival to a trauma centre”. One limitation I found in the study is how the use of violent trauma and Injury Severity Score could be arbitrary and changeable. Violent trauma was not defined, which could lead to misclassification. Moreover, ISS has been criticized on its limited discrimination power when scores exceed 15 and older patients. This could misdiagnose older victims with grievous injuries to have less significant scores. Moreover, the study did not define what is violent trauma. Although these problems were not addressed in the study, I would still give this report a 7/10, as it provided concise and easy to follow analysis and informative graphs and maps. 

###Other Presentation

#### The Effects of 'Alley-gating' in an English Town. 
by John Haywood, Paula Kautt, Andrew Whitaker
Presentation by Mielle Michaux
The objective was to access changes in burglaries resulting from the installation of alley in Oldham, North West England. The researchers used Police Report (6,193), Alley gate Location and time of installation, addresses of the area to evaluate the effectiveness gates to prevent burglary. The researchers used focus groups data to identify secondary effect of the installation of gates. Haywood, Kautt and Whitake argued that installation reduced victimization. 

My Thoughts:
I found this report interesting and innovative. It would a fascinating to have a similar project with alleys in Vancouver and having the project focus on the social aspects as well. 