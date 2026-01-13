---
layout: default
title: Add point data from a table
description: Learn how to turn a text table into a GIS point layer
permalink: /labs/lab06/part2
active: True
nav: False
multi: True
prev: part1
next: part3
---

# How to add point data from a table


1. Try adding the "TRI_sites_TX_UTM14N.csv" file the same way we added the first two layers, by dragging the file from the **Browser panel** to the **Layers Panel**

    ![](part2_images/user_cropped_screenshot.png)


2. Notice that no new data appeared on the map, and the new TRI layer has a **Table Icon** next to it. This is because this is a **CSV file** which stands for Comma Separated Values. Essentially this is a text file that represents a table of data

    ![](part2_images/screenshot.webp)


3. Right click "TRI_sites_TX_UTM14N" and select "Open Attribute Table". Now we can see the values of our table, which contains information about each Toxic Release Site. Notice that the table is **georeferenced**, meaning there is already location data (latitude and longitude) associated with each row of the table.

    ![](part2_images/screenshot_1.webp)


4. We do not see any new points on the map because QGIS does not automatically recognize this file a point layer. We need to specifically tell QGIS to plot this layer.

    Close the **Attribute Table Window** and open the **Data Source Manager**


5. Click "Delimited Text" in the **Data Source Manager** window

    ![](part2_images/user_cropped_screenshot_1.png)


6. Click "…" next to the **File name** field and navigate to your lab 6 data folder. Select the *TRI_sites_TX_UTM14N.csv* file

    ![](part2_images/user_cropped_screenshot_2.png)


7. In the **Geometry Definition** section, set the **X field** to the **LONGITUDE** column, set the **Y field** to the **LATITUDE** column, and set the **Geometry CRS** to **EPSG:3721 - NAD83(NSR2007) / UTM zone 14N**

    ![](part2_images/user_cropped_screenshot_3.png)


    <span class='alert'>Double and triple check your values in step 7! If these settings are incorrect, all of your calculations in this lab will be incorrect!
    </span>


8. Click **Add** then close the Data Source Manager window.


9. Zoom out on the map -- you can now see all the Toxic Release sites in Texas

    ![](part2_images/user_cropped_screenshot_4.png)


10. Remove the TRI **table** that we added in step 1. You should now only have three layers in your project

    ![](part2_images/screenshot_2.webp)

