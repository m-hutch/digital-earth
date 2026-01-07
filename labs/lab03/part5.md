---
layout: default
title: Filter Layer by Location
description: Learn how to filter a data layer by a defined location
permalink: /labs/lab03/part5
active: True
nav: False
multi: True
prev: part4
next: part6
---
# Filter Layer by Location

1. Click the check boxes next to "texas_roads/texas_roads.shp" and "texas_cities/texas_cities.shp" to make these layers visible

    ![](part5_images/ascreenshot.jpeg)


2. In the top menu, click **Vector**. Hover over **Research Tools** and click **Select by Location**

    ![](part5_images/screenshot.webp)


3. Select features from your **texas_cities** layer. Keep the **intersect** option checked. In the "By comparing to the features from" field, select the **texas_counties** layer (NOT the highlight_counties layer!)

    ![](part5_images/user_cropped_screenshot.png)


4. Click "**Run"** then click **"Close"**

    ![](part5_images/ascreenshot_1.jpeg)


5. Your selected features should now be visible in yellow.

    ![](part5_images/user_cropped_screenshot_1.png)


6. Right click the **texas_cities** layer and select Export &gt; **Save Selected Features As ...**

    ![](part5_images/ascreenshot_2.jpeg)


7. In the Save Vector Layer window, click "…"

    ![](part5_images/user_cropped_screenshot_2.png)


8. Navigate to your lab folder and save the file as **my_cities.shp.** click **Save.**

    ![](part5_images/ascreenshot_3.jpeg)


9. Keep all other defaults and click **OK**

    ![](part5_images/user_cropped_screenshot_3.png)


10. Click  the box next to "texas_cities/texas_cities.shp" to hide the layer. Now only cities in your selected county should be visible.

    ![](part5_images/ascreenshot_4.jpeg)


11. Repeat steps 2 through 10 on the **texas_roads** layer. It is OK if you have some roads that extend past your county boundaries, but roads that do not intersect with your county should not be visible

    ![](part5_images/ascreenshot_5.jpeg)
