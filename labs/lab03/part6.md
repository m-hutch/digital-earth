---
layout: default
title: Make a Population Density Map
description: Learn how to color your map according to population density
permalink: /labs/lab03/part6
active: True
nav: False
multi: True
prev: part5
next: part7
---
# Make a Population Density Map

1. Double click your Census Tract layer ("texas_ct_2020/texas_ct_2020.shp")

    ![](part6_images/user_cropped_screenshot.png)


2. In the **Symbology** section, change "Single Symbol" to **"Graduated"**

    ![](part6_images/user_cropped_screenshot_1.png)


3. In the **Value** box, select the **population** field

    ![](part6_images/ascreenshot.jpeg)


4. Click **"Classify"** to auto generate class categories. You are welcome to choose any **Mode** in order to make your map look how you think best communicates your data. Make sure you have at least 4 categories and no more than 8 categories

    ![](part6_images/ascreenshot_1.jpeg)


5. Click "Apply"

    ![](part6_images/ascreenshot_2.jpeg)


6. Take some time to look at your raw population map. Notice that the larger tracts tend to have more people living in them. It is very rare that you will ever need a raw population map as it does not give us much information. What would be much more useful is a **population density map**

    ![](part6_images/screenshot.webp)


7. In the Symbology window, click the Purple equation sign next to **Population**

    ![](part6_images/user_cropped_screenshot_2.png)


8. Click "/" to indicate division

    ![](part6_images/ascreenshot_3.jpeg)


9. Click the arrow next to **"Fields and Values"** then double-click **"AREA_SQMI".** Then click **OK**.

    ![](part6_images/ascreenshot_4.jpeg)


10. Click **"Classify"** then click **Apply**

    ![](part6_images/ascreenshot_5.jpeg)


11. Take some time to examine how your map has changed. Is it easier to identify where the most "Crowded" areas are now?


12. In the Layer Properties window, select a Color ramp that best illustrates your data

    ![](part6_images/ascreenshot_6.jpeg)


13. Note that in the U.S., **warm colors** (reds and oranges) are associated with crowdedness and high density while **cold colors** (blues and greens) are associated with low density. You may need to **invert your Color Ramp** to align these natural associations with your categories correctly.

    ![](part6_images/ascreenshot_7.jpeg)

