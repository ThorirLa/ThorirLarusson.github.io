---
layout: page
title: Exploring Drug and Narcotics Trends in San Francisco
permalink: /micro-project-social-data/

---

Welcome to our exploration of drug and narcotics trends in San Francisco! In this micro project, we delve into the San Francisco crime data spanning from 2003 to May 2018, aiming to uncover patterns and insights into drug-related incidents within the city.

### Understanding the Dataset

We begin by utilizing the San Francisco crime data available from [DataSF][crime-data]. This comprehensive dataset provides information on various crimes reported over the years, including details such as crime type, location, and time of occurrence.

### Visualizing Drug and Narcotics Trends

Our analysis kicks off with a captivating calendar plot showcasing drug and narcotic crime incidents over the past fifteen years. This visual representation allows us to identify trends and fluctuations in reported crime rates, providing valuable insights into temporal patterns.

![Calender plot for Drug and Narcotics](/images/calendar_plot_micro.png)

Upon close examination of the calendar plot, we observe intriguing fluctuations in crime rates, including a notable decrease in spikes around 2012. However, caution is warranted in interpreting recent years' data due to potential reporting delays or incomplete records.

### Investigating Historical Context

To contextualize our findings, we explore historical trends in drug epidemics in the United States, such as the crack cocaine and opioid crises. By drawing parallels between historical events and crime data trends, we gain a deeper understanding of the complex dynamics influencing drug-related incidents.

### Analyzing District-Level Patterns

Shifting our focus to district-level analysis, we present a choropleth map showcasing drug-related crimes across San Francisco districts. Unsurprisingly, the Tenderloin district emerges as a hotspot for such incidents, prompting further investigation into underlying factors contributing to its heightened crime rates.

[Crime by District Map](/html/map.html)

<!-- HTML block starts -->
<iframe src="{{ '/html/map.html' | prepend: site.baseurl }}" width="100%" height="500"></iframe>
<!-- HTML block ends -->

### Exploring Historical Trends by District

A compelling Bokeh plot illustrates the distribution of drug and narcotics crimes across districts over the fifteen-year period. This visualization confirms Tenderloin's dominance in drug-related incidents and highlights the evolving nature of crime patterns across different districts.

<!-- HTML block starts -->
<iframe src="{{ '/html/drug_crimes_by_year_and_district.html' | prepend: site.baseurl }}" width="100%" height="500"></iframe>
<!-- HTML block ends -->

### Conclusion and Future Directions

Our analysis offers valuable insights into drug and narcotics trends in San Francisco, shedding light on historical patterns and district-level dynamics. Moving forward, further exploration of historical data and correlation with socio-economic factors could deepen our understanding of the underlying drivers of drug-related crime.

Join us in unraveling the intricate tapestry of crime data as we continue to explore fascinating insights and implications for societal well-being.

[crime-data]: https://datasf.org/opendata/



