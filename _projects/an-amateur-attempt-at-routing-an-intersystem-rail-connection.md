---
layout: project-page
title: "An Amateur Attempt at Routing an Intersystem Rail Connection"
linkname: an-amateur-attempt-at-routing-an-intersystem-rail-connection
author: "Fletcher Berryman"
tagline: "My project was an attempt to use QGIS and satellite imagery to propose a feasible rail connection between the regional Metrolink system and municipal LA Metro system's Green Line in Greater Los Angeles (specifically Norwalk, CA)"
location:
    - place: Greater Los Angeles, California, USA
project-link:
    - href: https://docs.google.com/presentation/d/1c05a96F7YeMIl43fvk7YwsKUh94ytLFxVlQGhGkwGvk/edit
tags:
    - tag: public transit
    - tag:  transit mapping
    - tag:  routing
    - tag:  transit routing
    - tag:  los angeles
    - tag:  remote sensing
    - tag:  satellite imagery
    - tag:  georeferencing
    - tag:  public transit expansion
thumbnail-path: img/an-amateur-attempt-at-routing-an-intersystem-rail-connection/Ccw5SLW.png
img-folder: ../../img/an-amateur-attempt-at-routing-an-intersystem-rail-connection/
timestamp: 12/15/2018 11:01:39
---
Despite being the 2nd largest city proper (approx 4.9 million) in the US, second largest metro area (17 million) and 3rd largest city in world by GDP (over $1 trillion), the LA area lacks the public connectivity of cities such as New York or London. Meanwhile, its traffic is the nation’s worst, with high levels of car ownership and few alternatives. Though the actual track exists in mainly places for getting people around, its several systems (LA Metro, Metrolink, and Amtrak California) lack ideal integration.

LA Metro, the municipal rapid transit system, has in fact experienced a huge boost in public approval and use. Metrolink, the regional rail system, has significantly lower ridership. In several locations, the two systems nearly touch each other (and do connect at Union Station)

* LA Metro Daily Ridership: 359,061 (weekday)    # of lines: 6     # of stations: 93
* Metrolink Daily Ridership: 39,613 (weekday)      # of lines: 7     # of stations: 62

Transfers are already free between the two systems; however, gaps in crucial connection zones remain unfilled and make Metrolink inconvenient for most Southern Californians. 

![]({{ page.img-folder }}RBvp0L2.png)

I decided therefore to seek out locations best suited for building connections between the two systems. I initially expected to be investigating where might be ideal for connections; however, in researching the topic further it became clear that a specific gap around Norwalk, CA was the most suitable location. My project then took a drastic shift from what would have been investigating the causality of poor rail connectivity in certain areas (looking at demographics, history, etc) to instead using QGIS as a remote sensing tool with which to attempt some amateur routing.

I used Apple Maps, Google Maps, and the Transit App to examine existing distance/time commitments to travelling between the two stations with public transit.

![]({{ page.img-folder }}GqRZPkJ.png)

Using shapefiles from SCAG (Southern California Association of Governments), Los Angeles County and Orange County, I was able to load the respective networks’ polylines in QGIS. From there I used 3m resolution sample satellite imagery along with Google’s imagery basemap (available with QuickMapServices QGIS plugin).

Using QGIS I was able to “measure twice, cut once” and found a route through existing highway and street right-of-ways that would not require the demolition of any buildings (save for possibly one residential structure). Using QGIS and Google Earth I measured for the Minimum Railway Curve Radius in tight corners to determine whether light rail could make the turns and indeed the route was sufficient.

![]({{ page.img-folder }}kyWyqVc.png)

QGIS and the satellite imagery I imported were far more reliable than Google Earth of course and gave me the confidence to pull my various resources into one GIS. QGIS made selecting the relevant segments of both rail systems (using Select by Freehand) much easier than going into the attribute table, given the arbitrary nature of the cutoff points (I wanted to isolate the segments of rail that were being worked on for my maps so as to not confuse viewers by displaying the entirety of both systems.

Using American Community Survey information I was able to look at the population density of the census tracts around each of the 16 stations “cut off” from the LA Metro - Metrolink Green Line gap and found an average of ~ 6000 people lived within a mile of each. 

![]({{ page.img-folder }}4fFbUWr.png)

I naively assumed this would be a gargantuan endeavor and likely a pipe dream. My amateur analysis began with importing imagery into QGIS, mainly to measure the width of both medians and shoulders along existing interstate freeway segments and larger avenues in the area. I was pleasantly surprised to discover that connecting the railways would be, in the realm of public works projects, hardly intrusive at all! 

![]({{ page.img-folder }}pCFDyvW.png)

![]({{ page.img-folder }}pcP8LxS.png)
