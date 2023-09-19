# FLL-Gyro-And-Line-Follow-My-Blocks
*Update*: Sept, 2023 - New version of tools for Spike Prime 3.0 [MAR FLL Challeneg Tools - Spike Prime 3.0 2023](https://github.com/mar-fll-director/FLL-MAR-Tools-Spike-3.0-2023)

This repo will contain advanced FLL My Blocks for Line Follow and Gyro for EV3 and Spike Prime Robots
Important Note: The initial drop has problems in measuring distance. If it is working fro you keep going. If you want the distances to be more accurate, wait for the updates. 

This is all explained in a Google Slide deck [Gyro and Line Follow My Blocks Presentation](https://docs.google.com/presentation/d/1Vga1y9exY-jyWSlCoF_mPb3-asiujL25wlZJDBCBb4c/edit?usp=sharing). There is also a [Presentation Video](https://youtu.be/Y-mmc1qfdfc). This video has an index to the major sections. We suggest you view the **Setup The Environment** section at least once and then jump around as you need. 

The above presentsation is a deep dive into the details. There is a shorter presentation called [Help Students Use Line Follow and Gyro Tools](https://docs.google.com/presentation/d/1UHYsoMU4sQItIImVDW6JxholZiNHxqkA5VUVJfzfleM/edit?usp=sharing) that shows what you can do with the new "clean" demo free versions. The preso goes through adjustments you can do on the existing Line Follow and Gyro code or use the "clean" versions out of the box. It will show you how to use these as templates for your students to build their code with. 

We have added a [MAR Tools Line Follow and Gyro Q&A](https://docs.google.com/document/d/1ImXs9dXHien4vxTaczBTmVpKdwTA2yu8wNJbacyhVYc/edit?usp=sharing). This will defien the variables we use and report some Q&A we are receiving. 

## New Tool Spike Light Reflectivity Tester
This tool will allow you to test you light reflectivity in you location or at a competiton. Then you can make adjustments in the code settings. 
This is explained in the new [Help Students Use Line Follow and Gyro Tools](https://docs.google.com/presentation/d/1UHYsoMU4sQItIImVDW6JxholZiNHxqkA5VUVJfzfleM/edit?usp=sharing) presentation. 

Please let me know how it worked out for you. We will be opening the site to allow others to drop new tools of their own making. 

# Changes 
## Fixed bugs in cleaned up versions. Spike Demo Final V2 clean and EV3 Demo Final V2 clean -- Sept. 30, 2022 - 11:00 pm
Had **line waypoint reflectivity** and **line midpoint reflectivity** in incorrect places. Corrected and tested. 
Also added new tool for testing Spike light sensor reflectivity. In EV3, light reflectivity is on the dashboard. In Spike it is always color. Cannot test reflectivity like that. New **Tool Spike Light Reflectivity Tester.llsp** allows you to see Spike in reflectivity mode. See [Help Students Use Line Follow and Gyro Tools](https://docs.google.com/presentation/d/1UHYsoMU4sQItIImVDW6JxholZiNHxqkA5VUVJfzfleM/edit?usp=sharing) updated presentation for details. 

## Cleaned Up Versions, Spike Demo Final V2 clean and EV3 Demo Final V2 clean -- Sept. 29, 2022
These are cleaned up versions of the two programs. They do not have demo code in them. In addition all the chnages in the oroginal demo have been implemented. 
They are discuss in the new [Help Students Use Line Follow and Gyro Tools](https://docs.google.com/presentation/d/1UHYsoMU4sQItIImVDW6JxholZiNHxqkA5VUVJfzfleM/edit?usp=sharing) presentation.

## Addition of file, EV3 Demo Final V2 -- Sept. 21, 2022
This now follows the changes to the Spike Demo Final V2 as described in the presentaion. The video in the presentation does not use it so I could point out the difference between them. The V2 code works as good on EV3 as it deos on Spike. 

## Update to file, Spike Demo Final V2 -- Sept. 20, 2022
I changed the gyro turn to angle to use a preset turn speed called gyro turn speed max. This will make it so the turns are done slow enough to move the robot but not fast enough to throw off the gyro. I have found that I can induce an error in the gyro if I turn too fast. This prevents that problem.

Note: gyro turn speed min was renamed to gyro turn speed max. 

## New file, Spike Demo Final V2 -- Sept. 20, 2022
This version does not overwrite the old one so users can choose what to use. While not the most important part of this update, it does suggest that you use a more accurate representation of Pi like 3.141592 when calculating wheel circumference. When used your distance measurements will now be more accurate. 

This version contains a new important My Block called **gyro turn to angle**. This block accurately turns your robot to a desired angle. The presentation now contains all the descriptions of this My Block, under the Gyro discussion, and shows all the math. 

The My Blocks called **gyro drive to waypoint** and **gyro drive by distance** now call **gyro turn to angle** first and then continue as before. For **gyro drive by distane** this means the distance is now very accurate as the turn is not using any of the distance at that point. The my block **gyro drive by time** does not first use **gyro turn to angle**. The reasons are all explained in the updated presentation. 
