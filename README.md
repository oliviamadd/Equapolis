**Equapolis: A Tracker for Exposure and Awareness of Inequity in Toronto** 

Team: Angelina Abi Daoud, Olivia Maddigan, and Madinakhon Sulaymonova  

**Mission Statement**  

Toronto is Canada's largest city and serves as the capital of Ontario. This Canadian metropolis contains a population of over 2.9 million throughout its 140 neighbourhoods covering an area of 630.2 km2. Toronto represents Canada as a diverse world leader that roots for culture and ethnicity\[11\], however; the city has failed to take accountability regarding issues of neighbourhood equality. The city of Toronto specifically has come under fire for having high levels of disparity in quality of life between primarily white neighbourhoods and neighbourhoods where primarily visible minorities reside\[2\]. The 2019 Vital Signs of Toronto report confirmed that Toronto neighbourhoods are racially segregated, with the highest concentration of visible minorities living in the lowest-income neighbourhoods\[10\]. The reason for these disparities is a positive feedback loop of systemic racism. A single act of discrimination - whether it be someone failing to attain a job, a loan, or housing - can have a significant ripple effect, which affects the socioeconomic status of visible minorities to a great extent. This issue needs to be exposed and addressed, which is what Equapolis aims to do.   

It is 2021 and now more than ever, the federal, provincial, and municipal governments of Canada are facing scrutiny for institutional racism as outdated policies have negatively affected marginalized communities. From more well-known examples such as rural Indigenous communities going without clean water to more obscure but equally harmful examples such as black Torontonians being 20 times more likely to be shot by police than their white counterparts\[8\], it is clear that systemic racism is a problem here in Canada, no matter how “nice” our international reputation may be. Another result of inequity found within the population would be food insecurity. It affects almost 1 in 5 Toronto households. This is largely a byproduct of inequity among neighbourhoods. Essentially, the worse a family’s socioeconomic status is, the more likely they are to be severely food insecure, and in Toronto, these families happen to disproportionately be visible minorities. A lack of access to and awareness of food bank programs in Toronto have reduced the efficacy of community support efforts for those facing food insecurity. Equapolis considers these factors and makes food bank searching simple by providing the option to locate nearby local food banks\[5\]. This tool also provides information on areas where community support may be lacking.    

Our app aims to expose disparities between neighbourhoods in Toronto by creating a Neighbourhood Inequity Index (NEI) so that residents can see exactly what is happening in their own backyard. It aids in providing a broad quantitative assessment of wellbeing across the 140 neighbourhoods in Toronto \[3\]. It is a toolset to support the advancements of equity solutions. Our team believes that the term equity means ensuring both the wellbeing of individuals and communities, as well as moving towards closing racial gaps. By displaying the NEI on our application, we provide a snapshot into the state of each community and wellbeing of residents\[1\]. This must not be mistaken as an indicator of service inputs or population groups, rather the index is based on overall neighbourhood outcomes\[3\]. 
The purpose is to support community resilience in overcoming disparity among the overall population. We are aiming to reduce inequality by first exposing primarily racially-based inequality in Toronto\[4\]. We have created an app where users can see neighbourhood-based data pertaining to the quality of life of residents, and compare it to other datasets such as the concentration of visible minorities. Moreover, useful and critical information on food bank locations can be found in the app. Users can effectively use the app to identify disparity between neighbourhoods, in order to fully understand racial inequality and move towards addressing these issues in the community. We hope for a city in the near future where everyone is equal - an Equapolis.   

**App Description and Features**    

This app helps users identify communities in Toronto that are facing inequity compared to their neighbours. Using the Neighbourhood Inequity Index, you are able to examine neighbourhoods facing unequal circumstances, and view all the factors that lead to this inequality.   

_Search by Neighbourhood_    
Choose a neighbourhood from the drop-down menu to zoom in and display their characteristics   

_Compare Neighbourhoods_    
Display a column chart to compare inequity factors for every neighbourhood 

_Compare Layers_    
Swipe the center bar to compare the concentration of Visible Minorities with the Neighbourhood Inequity Index   
Note: Both layers must be turned on in Layers to compare them   

_Locate Nearby Food Banks_    
Enter your address or drop a pin to locate food banks near you and display their info Default search radius is 5 km, toggle the bar to increase or decrease it

**Calculations**   
Calculations for the Neighbourhood Equity Index (NEI) were done following the procedure outlined by the Social Policy Analysis and Research team for the City of Toronto (TSNS 2020 Methodological Documentation, 2014). All calculations were made using the Field Calculator in ArcGIS Pro. The NEI was calculated using 15 indicators that were weighted and combined to form the index. The 15 factors are outlined in Table 2 in the “Geospatial Open Data Sources” section. Because the 15 NEI indicators were presented in different units, they had to be standardized so that they all ranged from 0-1, where 1 is inequitable and 0 is equitable. For indicators where higher values indicate high inequity (such as Unemployment), the following formula was used for standardization: 

Standardized Value = Indicator Value - Min(Indicator Value)Max(Indicator Value) - Min(Indicator Value)    

Sample Calculation with Unemployment: Standardized Value = Indicator Value - Min(Indicator Value)Max(Indicator Value) - Min(Indicator Value)  

**Geospatial Open Data Sources**   

Table 1. Data for Visible Minorities Layer. 
| <b>Data Layer</b> | <b>Data Source</b> |
| --- | --- |
| % Visible Minorities | 2016 Neighbourhood Profiles (Toronto Open Data) |
| Population of each neighbourhood | 2016 Neighbourhood Profiles (Toronto Open Data) |
Table 2. Data used to calculate the Neighbourhood Equity Index (NEI). Data was compiled by Urban HEART@Toronto and the NEI was calculated by Team McRaster using ArcGIS Pro.
| <b>Data Layer</b> | <b>Data Source</b> |
| --- | --- |
| <b>Unemployment</b><br>(Number of unemployed persons age 15+) | 2011 National Household Survey |
| <b>Low Income</b><br>(Percentage of persons living below the after-tax low income measure) | Statistics Canada |
| <b>Social Assistance</b><br>(Percentage of persons who are recipients of Ontario Works, persons on ODSP participating in OW employment programs and non-OW persons receiving assistance with medical items) | Toronto Employment & Social Services |
| <b>High School Graduation</b><br>(Percentage of persons who are recipients of Ontario Works, persons on ODSP participating in OW employment programs and non-OW persons receiving assistance with medical items) | 2006 Census |
| <b>Marginalization Index</b><br>(A combined measure of 18 variables representing residential instability, ethnic concentration, dependency and material deprivation) | Ontario Marginalization Index |
| <b>Marginalization Index</b><br>(A combined measure of 18 variables representing residential instability, ethnic concentration, dependency and material deprivation) | Ontario Marginalization Index |
| <b>Post-Secondary Completion</b><br>(Percentage of persons age 25-65 with post secondary certificate, diploma, or degree) | 2011 National Household Survey |
| <b>Municipal Voting Rate</b><br>(Percent of eligible voters who voted in the last municipal election) | Toronto Election & Registry Services, Toronto Open Data |
| <b>Community Places for Meeting</b><br>(Average number of meeting places within a 10 minute walking distance measured from each residential block in the neighbourhoods [including libraries, recreation facilities, and places of worship]) | Toronto Open Data |
| <b>Walkability</b><br>(A walkability score between 0 (not very walkable) and 100 (very walkable)) | Walkscore.com |
| <b>Healthy Food Stores</b><br>(The average number of healthier food stores within a 10 minute walking distance from each residential block in a neighbourhood) | Toronto Open Data, Toronto Dinesafe |
| <b>Greenspace</b><br>(Average amount of green space (including parks and public areas) per km2 in a 1 km circular buffer from each residential block in the neighbourhood) | DMTI (University of Toronto) |
| <b>Premature Mortality</b><br>(Age-adjusted number of deaths under age of 75 per 100,000 population age under 75) | Ontario Mortality Data 2005- 2009, Ontario Ministry of Health and Long-Term Care |
| <b>Mental Health</b><br>(Percentage of those age 20+ reporting very good or excellent mental health) | 2005-2011 Canadian Community Health Survey |
| <b>Preventative Hospitalizations</b><br>(Age and sex adjusted number of ambulatory care sensitive condition hospitalizations per 100,000 population) | 2009-2011 Discharge Abstracts Database, Canadian Institute for Health Information |
| <b>Diabetes</b><br>(Age and sex adjusted number of persons age 20+ with diabetes per 100 population) | Ontario Diabetes Database, Ontario Registered Persons Database, Ontario Ministry of Health and Long-Term Care |

 _Note: The Food Banks layer was created by Team McRaster._    
 
 **Reference**   
 
 \[1\] https://nationalequityatlas.org/research/index-findings   
 \[2\]https://www.thestar.com/news/gta/2018/09/30/toronto-is-segregated-by-race-and-income-and-the-numbers-are-ugly.html   
 \[3\]https://www.toronto.ca/wp-content/uploads/2017/11/97eb-TSNS-2020-NEI-equity-index-methodology-research-report-backgroundfile-67350.pdf   
 \[4\] https://www.toronto.ca/legdocs/mmis/2014/cd/bgrd/backgroundfile-67382.pdf   
 \[5\]https://www-cambridge-org.libaccess.lib.mcmaster.ca/core/journals/public-health-nutrition/article/assessing-the-relevance-of-neighbourhood-characteristics-to-the-household-food-security-of-lowincome-toronto-families/7CCCA5930BA7171F2C893188671BEC3F   
 \[6\]https://datacommons.org/place/wikidataId/Q172?utm\_medium=explore&mprop=count&popt=Person&hl=en   
 \[7\]https://www.toronto.com/news-story/10111865-this-is-a-fact-systemic-racism-makes-life-harder-for-many-ontarians/   
 \[8\] https://globalnews.ca/news/7029694/canada-systemic-racism/   
 \[9\]https://globalnews.ca/news/7015522/black-neighbourhoods-toronto-coronavirus-racism/   
 \[10\] https://torontofoundation.ca/wp-content/uploads/2019/10/VitalSigns2019.pdf. 
 \[11\] https://www.canadapopulation.net/toronto-population/   
 Video and Audio references:   
 Stock footage credits: https://www.pexels.com/videos/ https://www.videvo.net/ Background music credits: https://www.bensound.com   
 Image credits to: https://unsplash.com/photos/VviFtDJakYk (Matthew Henry) https://unsplash.com/photos/-Y9XT1-5LL8 (Justin Lawrence)  
