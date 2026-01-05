---
layout: default
title: Lab 2 - Introduction to QGIS
description: Learn how to import and display data using QGIS
permalink: /labs/lab02/start
active: True
nav: False
multi: True
next: part1
prev: Null
---
# Lab 2 - Introduction to QGIS
*Estimated time to complete: 2 hours*

## Goals:
- Learn about the basic functions in QGIS
- Customize vector layer symbology and labels
- Create a professional map layout

## Key Performance Indicators:
These indicators are used to assess student performance.

- **KPI 1**: Imports data to a QGIS project an appropriately orders layers to make all relevant data visible
- **KPI 2**: Filters vector layers by attributes
- **KPI 3**: Selects features by attributes and exports selection to a new vector layer
- **KPI 4**: Applies custom single and category-based symbology
- **KPI 5**: Applies formatted labels to a vector layer
- **KPI 6**: Edits layout size and color properties
- **KPI 7**: Adds formatted text and dynamic text elements to a layout
- **KPI 8**: Add critical map elements (scale, direction, legend) to a layout and formats appropriately
- **KPI 9**: Add and format data table in a layout

## Requirements:
- Microsoft Word
- QGIS
- Computer with an Internet connection
- Data files:
    * Texas_Cities.gpkg
    * Texas_State_Boundary.gpkg
    * TxDOT_Roadways.gpkg

## Optional
 - A computer mouse (separate from a laptop track pad) for easy map navigation


## Lab Overview
There are **ten** parts to this lab:

* Creating a QGIS project & opening existing projects
* Adding data to a QGIS project
* Using the Statistics Panel & Filtering data layers
* Selecting by attribute & exporting selections
* Single & Category-based Symbology
* Adding labels
* Creating a map layout
* Adding a data table to a layout
* Exporting a layout as a high-res image
* Submit your lab report

Please complete each part *in order* and submit your lab report before the due date.

The lab will be graded based on the Key Performance Indicators (KPIs):

|KPI| Description | Total Points  Possible |
|---|:--|--:|
|//	|COMPLETION OF THIS CHECKLIST|	2|
|//	|First and Last name written in the header of your lab report|2|
|//	|Map layout is submitted as a high-resolution image file, professionally formatted and generally legible|6|
|1|	Texas boundary, roads, and cities layers are visible on the map layout|10|
|2a|	Only US and Interstate Highways are visible on the roads layer	|5|
|2b|	Only cities with a 2022 population >100,000 are visible on the cities layer	|5|
|3|	Major cities with a 2022 population >500,000 are represented by their own data layer	|10|
|4a|	US highways and Interstate highways are represented in two different colors|5|
|4b| Large cities and Major cities are represented by appropriately different symbols |5|
|5| Major cities are labeled by city name using size 12 text in a non-default legible font with a text buffer|10|
|6| Layout is a 8-inch by 8-inch square and has an appropriate background color other than white |5|
|7a| Title is legible and appropriately named  in size 36 text using a non-default font |2|
|7b| Data source, map author name and date are in size 14 text using the same font as the cites labels|3|
|7c| CRS name is visible using dynamic text feature, in size 12 text using the same font as the map author name and date|5|
|8a| Scale bar is appropriately sized (in miles)|2|
|8b| North arrow is appropriately sized|3|
|8c| Legend is appropriately sized  displaying only the visible layers and appropriately labeled layer names using size 14 text in the same font as the city names|5|
|9a| Data table of city names and population references the major cities layer and is appropriately sized using size 14 text in the same font as the city names|5|
|9b| Data table headers are visually distinct from the table data, and numbers are formatted with commas |5|
|---|---|---|
| |**Total**| 100|

## Set up material
Before starting, make sure to download:
- [Lab02_Report.docx]({{'/labs/lab02/Lab02_Report.docx' | relative_url}})
- [data.zip]({{'/labs/lab02/data.zip' | relative_url}})
- [Layout_example]({{'/labs/lab02/Layout_example.png' | relative_url}}){:target="_blank"} 

Create a folder called `lab02` in your `digital-earth` folder on your computer and save the report and data to this folder.

After you have saved both files to your `lab02` folder, extract (unzip) the compressed `data` folder before starting the lab.