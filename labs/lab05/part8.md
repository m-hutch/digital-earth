---
layout: default
title: Bonus -  Make a heat map
description: ...
permalink: /labs/lab05/part8
active: True
nav: False
multi: True
prev: part7
next: part9
---
# Bonus: Make a heat map from GPS data
This section is optional. These instructions describe how to make a heat map of open-source GPS usage in your study area, similar to the public Snap Map on Snapchat.

<span class='alert'>This bonus exercise is easier to do in **light mode**. If your computer is in dark mode, we recommend switching to light mode just for this portion of the lab. You would need to do this in your computer's settings, not in QGIS. Close and reopen QGIS after you switch to open QGIS in light mode.</span>


1. Click "Search NextGIS QMS"

    ![](part8_images/user_cropped_screenshot.png)


2. Add the OpenSTrettMap GPS traces layer

    ![](part8_images/user_cropped_screenshot_1.png)

3. You should see the available GPS traces appear on your map. Be patient as it may take a few minutes to load. Uncheck your "satellite_image" layer to see the traces better.

    ![](part8_images/user_cropped_screenshot_2.png)

    <span class='tip'>If there are no available GPS traces at the location you chose for your postcard, you can choose another location to do the bonus map for. All you need to do is add back the Esri World Imagery layer from QMS as your base map so that you have satellite imagery of the new area; you do not need to re-do the main part of the lab.
    </span>


4. With **only the GPS traces layer visible**, click **Project &gt; Import/Export &gt; "Export Map to Image…"**

    ![](part8_images/user_cropped_screenshot_3.png)


5. In the "Save Map as Image" window, in the **Extent section** choose to **Calculate from Layer &gt; Satellite_image**. This insures we only save the GPS traces for our area of interest instead of the whole world.

    ![](part8_images/ascreenshot.jpeg)


    <span class='alert'>If you are using a different location for the bonus than the location you made the postcard about, choose **Map Canvas** extent instead.</span>


6. save the images as **gps_traces.TIF**  in your **lab 5 folder**

    ![](part8_images/user_cropped_screenshot_4.png)


7. If you saved "gps_traces.tif" in the same folder as your QGIS project, you can easily add it by dragging it from the **Browser** panel to the **Layers** panel.

    ![](part8_images/user_cropped_screenshot_5.png)


    <span class='tip'>If you can't find your **Browser** or **Layers** panel, you can reopen them by clicking **View &gt; panels** and then selecting the missing panel
    </span>


8. Turn off your  "OpenStreetMap GPS traces" layer. You should still see your GPS traces layer for your original map extent.

    ![](part8_images/user_cropped_screenshot_6.png)


9. Notice how our **gps_traces** layer has **three bands** (Red, Green, and Blue). Because we want to make a single-layer heatmap, we need to flatten this layer into a single-band **Pseudo-Color Table (PCT).** Click **Raster&gt; Conversion&gt; "RGB to PCT…"**

    ![](part8_images/user_cropped_screenshot_7.png)


10. In the **Raster Conversion - RGB to PCT** window, make sure your **Input layer**  is set to **gps_traces** and your **Number of colors** is set to **5**. If your gps_traces layer is very faint (similar color to your background) you may need to choose a higher number of colors to make sure you get all the points. (any number from 5 to 12 is fine).

    ![](part8_images/user_cropped_screenshot_8.png)


11. Instead of saving to a temporary file, click the three dots "..." and select **Save to File**.

    ![](part8_images/screenshot.webp)


12. Name your file **gps_flattened.tif** and save it in your Lab 5 folder. Click **Save**.

    ![](part8_images/ascreenshot_1.jpeg)


13. Go back to the **Raster Conversion-RGB to PCT** window (it may have minimized itself but it should still be open) an. Make sure **"Open output file after running algorithm"** is selected and click **Run**

    ![](part8_images/user_cropped_screenshot_9.png)


14. When the job says "Complete" at the bottom of the window, click **Close**.

    ![](part8_images/user_cropped_screenshot_10.png)


15. Click the arrow next to "gps_flattened" to expand the layer. You should see a list of colors that the conversion process detected.

    ![](part8_images/ascreenshot_2.jpeg)


16. Find the number that corresponds to the square that most closely matches the background color. In this example it is **4**, **but it may be different in your project**. If there are more squares than one that look like a matching color, note down all the corresponding numbers that you think might be the background color.

    ![](part8_images/ascreenshot_3.jpeg)


17. Click Processing &gt;  "Toolbox"

    ![](part8_images/screenshot_1.webp)


18. In the Processing Toolbox pane, search "Raster pixels to points" and select the corresponding tool

    ![](part8_images/ascreenshot_4.jpeg)


19. In the **Vector Creation** window, make sure the **gps_flattened** layer is selected.

    Under **Vector points**, click the three dots "..." and select **Save to File**

    ![](part8_images/ascreenshot_5.jpeg)


20. Save the file as **gps_points.gpkg** in your Lab 5 folder

    ![](part8_images/ascreenshot_6.jpeg)


21. Make sure "Open output file after running algorithm is checked and click **Run**.

    ![](part8_images/user_cropped_screenshot.webp)


22. When the process finishes, click **Close**.


23. The new points layer will appear as a totally blank layer. This is because there are so many points, we are only seeing the outlines of the points.

    Double click "gps_points" layer to edit the symbology

    ![](part8_images/ascreenshot_7.jpeg)


24. Change the symbology to **categorized** and the value to **VALUE**. Click **"Classify" to** to auto-generate categories.

    Make sure that you see the background **Value** you wrote down in step 16. If you don't, add a new category with the (+) button where the value is equal to the background value you wrote down.

    ![](part8_images/user_cropped_screenshot_1.webp)


    <span class='alert'>The **Symbol** colors in the Symbology layer are randomly assigned, they have no correlation to the pixel colors we examined in step 16.
    </span>


25. Click **OK** to apply the symbology and close the properties window.


26. Uncheck the background category number. you should now see dots that trace out the original GPS traces layer we started with.

    ![](part8_images/ascreenshot_8.jpeg)


27. Right click on the **gps_points** layer and click **Filter**

    ![](part8_images/ascreenshot_9.jpeg)


28. Filter out the background **VALUE** by using the != sign, which means "not equals"

    In this example the background value is **4**, but **you should use your corresponding background value**

    ![](part8_images/ascreenshot_10.jpeg)


29. Turn on the category you disabled in step 26. If your filter was successful, you should see **no change** in the map preview.

    ![](part8_images/ascreenshot_11.jpeg)


30. Reopen the Symbology for the **gps_points** layer and change it to **Heatmap**

    ![](part8_images/ascreenshot_12.jpeg)


31. Change the **Color Ramp** to **Turbo**.

    ![](part8_images/ascreenshot_13.jpeg)


32. Click the color bar to edit the **Color ramp**

    ![](part8_images/user_cropped_screenshot_2.webp)


33. Change **Color 1** to **Transparent** then click **OK**

    ![](part8_images/ascreenshot_14.jpeg)


34. Change the **Opacity** to about **50%** then click **OK**

    ![](part8_images/user_cropped_screenshot_3.webp)


35. Turn off the intermediary gps layers we made and turn on your satellite imagery layer

    ![](part8_images/ascreenshot_15.jpeg)


36. Make a **New Print Layout** called "bonus heatmap - \[LOCATION NAME\]" replacing "\[LOCATION NAME\]" with the name of your location.


37. Add a new map and adjust the frame so that it takes up the whole page. Interact with the map to zoom in and adjust as necessary so that there is no blank space.


38. Export the layout as a jpeg image and upload it as an additional file with your postcard and lab checklist.

    ![](part8_images/screenshot_2.webp)