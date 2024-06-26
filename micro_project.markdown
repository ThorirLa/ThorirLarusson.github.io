---
layout: page
title: Micro Project in social data
permalink: /Micro Project/
---

A little bit about our project, we are going to use the San Francisco crime data from 2003 to May 2018. Here is the link to the [crime data][crime-data]. This dataset contains information about various crimes reported in San Francisco over several years. Each entry includes details such as the type of crime, the location where it occurred, and etc. By analyzing this dataset, we can provide insights into trends and patterns in criminal activities over time and space within the city.

Over the past few weeks, we have been closely studying this dataset and have discovered many interesting insights into crime-related issues in San Francisco. However, I've always found the topic of drugs and narcotics in the United States fascinating. There have been numerous epidemics in the country's history, such as the [crack cocaine][crack-cocaine] epidemic, the [OxyContin epidemic][opioid-epidemic] , and today we face the [fentanyl epidemic][opioid-epidemic]. For this micro project, we aim to delve into drug and narcotics data from 2003 to 2018 to uncover interesting patterns and connections and maybe we can related to these epidemics. Let's begin by plotting the crime data concerning drugs and narcotics over the past years.

![Calender plot for Drug and Narcotics](/images/calander_plot_micro.png)

The calpolt offers a visual representation of drug and narcotic crime incidents over a period of fifteen years. This type of plot allows us to quickly discern patterns and trends over time, with darker spots indicating higher reported crime rates and lighter spots indicating lower rates.

Upon examining the calendar plot, it is intriguing to note the significant drop in crime spikes in 2012, suggesting a decrease in the frequency of drug/narcotic crimes. However, the lighter color in more recent years may be attributable to incomplete data, warranting caution in interpretation. The possibility of fewer crimes or data inaccuracies, possibly due to reporting delays, underscores the need for careful analysis.

Furthermore, the plot reveals that the majority of drug-related crimes occurred between 2007 and 2009, coinciding with the global financial crisis.

Upon further investigation, I observed spikes in drug overdoses around 2010, correlating with the rise in heroin overdose deaths, and another surge in synthetic opioid overdose deaths in 2013. This discrepancy between decreasing crime rates and increasing overdoses raises questions. One would expect a correlation between overdose rates and crime rates, yet the data suggests otherwise. This anomaly warrants further exploration to understand the complex dynamics at play.

For additional context, consider the image and link showcasing the waves of the [opiod overdoses][opioid-epidemic]:
![opioid](/images/opiod.png)

Additionally, in an [article][most-common-drug] I found, the most common drug charge is the possession of marijuana, typically classified as a misdemeanor. This observation could potentially correlate with the decrease in reported drug-related incidents. Given that California legalized the possession of marijuana in 2018, it's possible that the popularity of marijuana wasn't being accurately reported in the later years, thus contributing to the apparent decline in drug-related incidents. While various factors could explain the observed decreases, this aspect is nonetheless intriguing.


Now let's shift our focus to district-level analysis, we present a choropleth map showcasing drug-related crimes across San Francisco districts. This exploration may offer insights into where the highest concentration of related crimes occurs within the districts. With this knowledge, we can allocate additional police resources to those areas accordingly.

<!-- HTML block starts -->
<iframe src="{{ '/html/map.html' | prepend: site.baseurl }}" width="100%" height="500"></iframe>
<!-- HTML block ends -->

The choropleth mapbox plot clearly indicates that the district with the highest number of drug-related crimes is Tenderloin. Therefore, we decided to investigate why Tenderloin is such a hotspot. As expected, [Tenderloin][tenderloin] emerges as the most dangerous district in San Francisco, where the highest number of homeless individuals and crimes are reported. Utilizing this data, we can strategically increase police patrols in these areas to mitigate drug-related incidents.

Additionally, employing tools such as heatmaps, as demonstrated below, enables us to analyze crime patterns and determine optimal patrol placement:

<!-- HTML block starts -->
<iframe src="{{ '/html/drug_arrest_map.html' | prepend: site.baseurl }}" width="100%" height="500"></iframe>
<!-- HTML block ends -->

Social visualization techniques can significantly contribute to reducing crime rates by identifying high-risk areas. This approach is known as predictive crime analysis, which you can read more about [here][Predictive-policing].

After observing the prevalence of drug and narcotics crimes in the Tenderloin district, we wondered whether this trend has persisted over the past 15 years. Below, we present a bokeh plot illustrating the distribution of such crimes across districts during this period. This visualization allows us to track changes in each district over time.

<!-- HTML block starts -->
<iframe src="{{ '/html/drug_crimes_by_year_and_district.html' | prepend: site.baseurl }}" width="100%" height="500"></iframe>
<!-- HTML block ends -->

The compelling bokeh graph confirms Tenderloin's dominance in drug and narcotics-related crimes, which aligns with expectations. Interestingly, upon excluding Tenderloin from the analysis, we notice that the Southern district follows closely behinde and even in 2017 it is basically even. It would be fascinating to explore additional historical data, such as during the onset of the cocaine crack epidemic, to further understand the evolution of district dynamics over time. Nonetheless, delving into the dataset of drug and narcotics crimes in San Francisco presents endless opportunities for analysis and the discovery of intriguing insights.




[crime-data]: https://datasf.org/opendata/
[crack-cocaine]: https://en.wikipedia.org/wiki/Crack_epidemic_in_the_United_States
[opioid-epidemic]: https://en.wikipedia.org/wiki/Opioid_epidemic_in_the_United_States
[most-common-drug]: https://www.roselegalservices.com/what-drug-charges-are-most-common/
[tenderloin]: https://en.wikipedia.org/wiki/Tenderloin,_San_Francisco#:~:text=Part%20of%20the%20western%20extent,and%20crime%20in%20the%20city.
[Predictive-policing]: https://en.wikipedia.org/wiki/Predictive_policing


