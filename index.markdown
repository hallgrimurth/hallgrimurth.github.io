---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default

---

# **Drug Crime in San Francisco - A Closer Look at the Tenderloin**

## About This Project

This site presents a data story created as part of the course **02806 Social Data Analysis and Visualization** at the Technical University of Denmark (DTU).

The story investigates patterns in **drug-related crime in San Francisco**, with a particular focus on the **Tenderloin district** over time. Emphasis is placed on creating a **visual narrative** grounded in public data.

All figures, analyses, and visualizations were created using publicly available crime data from [SF OpenData](https://datasf.org/opendata/), with records dating back to **January 2003**.

### Authors

- **Daniel Diamant**  
- **Hallgrímur Thorsteinsson**
- **Ha My Ngo**

Group 29, Spring 2025

---

## **Mapping Drug Crime Patterns Across San Francisco**

In this post, we explore the spatial distribution of drug-related crimes across San Francisco using a series of **choropleth maps**. The data focuses on the years **2016 to 2024**.

Below is a multi-panel figure showing yearly distributions:

![Choropleth Map of Drug Crimes](/assets/img/choropleth_map_2.png)

### **Key Observations**
- **Tenderloin** remains the most consistently affected district throughout the time range.
- Adjacent districts like **Southern** and **Mission** show modest but visible activity.
- During **2020–2021**, a slight drop is visible, which may reflect the impact of the COVID-19 pandemic on policing or reporting. Interestingly, while the pandemic slowed down law enforcement activity and disrupted city services, it also opened up space for other forms of neighborhood expression. As reported by [The Bold Italic](https://thebolditalic.com/in-defense-of-the-tenderloin-san-francisco-2ad189635485), **2020 and 2021 saw a rise in mural creation**, local artists used the moment to turn the neighborhood into a canvas.
- In **recent years (2022–2024)**, case numbers appear to rise again, with the Tenderloin still dominating the map in intensity.

### **But why does the Tenderloin stay so persistent — and different?**

Some answers can be found in San Francisco's urban policy history. According to a [KQED article](https://www.kqed.org/news/11665527/why-hasnt-the-tenderloin-gentrified-like-the-rest-of-san-francisco), the Tenderloin is **unusual among city neighborhoods** in that it has not followed typical gentrification patterns is by design.

Several key policies and conditions have helped **preserve affordability and limit speculative development** in Tenderloin. When land was still cheap, nonprofit organizations acquired a large amount of property in the Tenderloin and have kept much of it in use for affordable housing. Since 1985, buildings over 13 stories have been banned, discouraging luxury high-rise development and maintaining the district's older architectural character. The buildings are often without private kitchens or bathrooms, are legally protected, making them unattractive to wealthier renters and preserving low-income housing stock. Much of the Tenderloin is classified as a historic district, which further limits redevelopment and prevents major architectural transformation.

All of this means the Tenderloin hasn't undergone the same physical, demographic, or economic shifts as other neighborhoods — and may help explain why drug-related activity remains **concentrated and visible** here.

-----------
### **A Closer Look at Drug Cases per District**

The bokeh bar chart below visualizes the number of **drug-related incidents** from the districts of the map. The data is stacked by district, making it easy to observe both trends. When you hover over a bar in the chart you can see the percentage of the total drug cases in s.f happen Tenderloin.

<iframe src="/assets/drug_incidents_by_district.html" title="Interactive Bokeh Plot of Drug Crimes" style="width:100%; height:600px; border:none;"></iframe>

Some key takeaways from the visualization:

- As we saw earlier **Tenderloin** stands out dramatically across all years. From the mid-2000s to 2010, the number of drug-related incidents in this district surged, peaking at nearly **5,000 cases per year**. This trend saw a decline in the mid-2010s but has **resurged again after 2018**, this might be because of the rise in popularity of fentanyl that happened at that time [Fentanyl epidemic hits the U.S. West Coast"](https://www.sciencedirect.com/science/article/abs/pii/S0955395921003078).
- Other districts such as **Southern**, **Mission**, and **Bayview** show consistent but comparatively lower levels of activity. While their trends also vary year to year, none come close to the persistent intensity seen in the Tenderloin.
- Not only does the Tenderloin consistently report the highest number of cases, but its **share of the total drug-related incidents citywide has also grown significantly**. In recent years, **over 50%** of all reported drug incidents in San Francisco have occurred in the Tenderloin.

----------------------
### **Crime Resolution Effectiveness: The Tenderloin Paradox**

Our analysis of San Francisco crime data reveals a surprising insight about the Tenderloin district. Despite being known for high crime rates and limited gentrification compared to other neighborhoods, the Tenderloin actually demonstrates better crime resolution rates than many other districts in the city.

This finding challenges conventional assumptions about policing effectiveness in high-crime areas. While one might expect a struggling neighborhood to have worse crime resolution outcomes, our data visualization shows the opposite – the Tenderloin's resolution rates stand notably higher than districts with lower overall crime rates.

<iframe src="/assets/sf_crime_resolution_map.html" title="Interactive Map of Crime Resolution Rates" style="width:100%; height:600px; border:none;"></iframe>

The explanation emerges when we examine the types of crimes that occur in each district. While most San Francisco neighborhoods show theft as their predominant crime category (around 50% of all reported incidents), the Tenderloin displays a markedly different pattern. In this district, drug and narcotic-related offenses constitute the largest category at 31.7% of total reported crimes.

This difference in crime composition directly impacts resolution statistics. Drug crimes possess inherent characteristics that make them more readily resolvable:

1. They typically involve direct observation by officers, with perpetrators caught in the act
2. Unlike property crimes where perpetrators may have fled, drug crimes generally require the offender's presence
3. The evidence (illicit substances) is typically found on the person being arrested

In essence, drug crimes are often "pre-solved" upon discovery – when law enforcement identifies a drug crime, they typically already know who committed it. This contrasts sharply with crimes like theft or burglary, where identifying and apprehending suspects presents greater challenges.

The Tenderloin holds a unique position among San Francisco’s urban districts, remaining less gentrified while experiencing higher crime rates. This does not appear to be due to ineffective policing and may instead stem from structural factors. The district’s resistance to gentrification—maintained through nonprofit property ownership, building height restrictions, legally protected single-room-occupancy housing, and historic district classification—has helped preserve its distinctive character and demographics. At the same time, the prevalence of drug-related crimes, which are easier to resolve, contributes to a paradox where the area reports both high crime rates and a higher resolution rate compared to other districts.

*Note: Hover over each district on the map to see detailed crime category distributions.*





## **References**

[KQED article](https://www.kqed.org/news/11665527/why-hasnt-the-tenderloin-gentrified-like-the-rest-of-san-francisco)

[The Bold Italic](https://thebolditalic.com/in-defense-of-the-tenderloin-san-francisco-2ad189635485)

[Fentanyl epidemic hits the U.S. West Coast"](https://www.sciencedirect.com/science/article/abs/pii/S0955395921003078)

---------

## **Contributions**

- **Hallgrímur Thorsteinsson** – A Closer Look at Drug Cases per District / Website 
- **Daniel Diamant** – Crime Resolution Effectiveness section
- **Ha My Ngo** – Mapping Drug Crime Patterns Across San Francisco section
