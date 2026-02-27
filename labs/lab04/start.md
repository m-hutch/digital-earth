---
layout: default
title: Lab 4 - Digitization
description: Learn how to digitize features in QGIS
permalink: /labs/lab04/start
multi: True
active: True
nav: False
prev: NULL
next: part1
---
# Lab 4 - Digitization
*Estimated time to complete: 2 hours*  

## Goals 

- Learn about georeferenced images
- Digitize a feature using a referenced image
- Digitize unique features with attributes
- Apply symbology and labels using digitized feature's attributes

## Key Performance Indicators
- **KPI 1**: Digitize feature from a georeferenced image
- **KPI 2**: Create Point Features
- **KPI 3**: Create Line Features
- **KPI 4**: Create Polygon Features
- **KPI 5**: Apply Complex Labeling
- **KPI 6**: Apply Categorical Symbology
- **KPI 7**: Add a base map
- **KPI 8**: Produce a professional, high-quality layout

## Requirements
- Microsoft Word
- QGIS
- Data Files from eLearning:
    - universal_frisco_map_WFAA.tif
    - universal_frisco_map_WFAA.tif.aux.xml

## Lab Overview

There are **seven** parts to this lab:
- Using georeferenced images
- Using Scratch layers
- Digitizing Features
- Applying Symbology
- Using the QMS Plugin
- Creating a map layout
- Submit your lab

Please complete each part in order and submit your lab report before the due date.

The lab will be graded based on the Key Performance Indicators (KPIs):

|KPI | Requirements	| Points | 
|---|---|---|
|//	| Completion of this Checklist	|2|
|//	| First and Last name written in the header of your lab report	| 2 |
|//|	Map layout is submitted as a high-resolution PDF file, professionally formatted and generally legible	|6|
|1| Digitize feature from a georeferenced image: Park Footprint is visible and closely matches the shape and location of the provided reference image |10|
|2| Create Point Features: At least two guest entrances and one staff entrance are visible, appropriately named and labeled |10|
|3| Create Line Features: At least two distinct walking paths are visible, appropriately named and labeled |10|
|4a| Create Polygon Features: At least two named parking lots are indicated on the map |10|
|4b| Create Polygon Features: At least ten named attraction areas are indicated on the map |10|
|5a| Apply Complex Labeling: All digitized features are labeled by name in legible text |5|
|5b| Apply Complex Labeling: Parking lot labels include the number of parking spots clearly labeled |5| 
|6a| Apply Categorical Symbology: All legend layers are appropriately named |5|
|6b| Apply Categorical Symbology: Attraction Areas are colored by four or more themes, which are indicated in the legend |5|
|7| Add a base map: base map is visible on the map|10|
|8a| Appropriately sized scale bar (in YARDS) & North Arrow | 2|
|8b| Appropriately formatted Legend |2|
|8c| Appropriate Title |2|
|8d| Coordinate Reference System (CRS) Name |2|
|8e| Name & Date |2|



## Set Up

Before starting, make sure to download:

- [Lab04_Report.docx]({{'/labs/lab04/Lab04_Report.docx' | relative_url}}){:target="_blank"}
- [data.zip](https://utdallas.box.com/s/pumkf7c997t6ykn2eksgglub2s8fjosm){:target="_blank"}
- [Layout_example]({{'/labs/lab04/Example_Layout.jpg' | relative_url}}){:target="_blank"} 

Create a folder called `lab04` in your `digital-earth` folder on your computer and save the report and data to this folder.

After you have saved both files to your `lab04` folder, extract (unzip) the compressed data folder before starting the lab. 

Before proceeding, familiarize yourself with the Universal Studios theme park in Frisco, Texas:
[WFAA Report](https://www.wfaa.com/article/news/local/how-will-traffic-flow-in-out-of-new-universal-studios-theme-park-frisco/287-0cda26a2-7219-4797-8d45-89d7ebfe4440){:target="_blank"}

Use the [Blank Park Footprint]({{'/labs/lab04/Blank_Park_Footprint.pdf' | relative_url}}){:target="_blank"} to sketch out your ideas for a theme park design.
