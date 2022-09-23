# FLL-Gyro-And-Line-Follow-My-Blocks
This repo will contain advanced FLL My Blocks for Line Follow and Gyro for EV3 and Spike Prime Robots
Important Note: The initial drop has problems in measuring distance. If it is working fro you keep going. If you want the distances to be more accurate, wait for the updates. 

This is all explained in a Google Slide deck [Gyro and Line Follow My Blocks Presentation](https://docs.google.com/presentation/d/1Vga1y9exY-jyWSlCoF_mPb3-asiujL25wlZJDBCBb4c/edit?usp=sharing). There is also a [Presentation Video](https://youtu.be/Y-mmc1qfdfc). This video has an index to the major sections. We suggest you view the **Setup The Environment** section at least once and then jump around as you need. 

Please let me know how it worked out for you. We will be opening the site to allow others to drop new tools of their own making. 

## Addition of file, EV3 Demo Final V2 -- Sept. 21, 2022
This now follows the changes to the Spike Demo Final V2 as described in the presentaion. The video in the presentation does not use it so I could point out the difference between them. The V2 code works as good on EV3 as it deos on Spike. 


## Update to file, Spike Demo Final V2 -- Sept. 20, 2022
I changed the gyro turn to angle to use a preset turn speed called gyro turn speed max. This will make it so the turns are done slow enough to move the robot but not fast enough to throw off the gyro. I have found that I can induce an error in the gyro if I turn too fast. This prevents that problem.

Note: gyro turn speed min was renamed to gyro turn speed max. 


## New file, Spike Demo Final V2 -- Sept. 20, 2022
This version does not overwrite the old one so users can choose what to use. While not the most important part of this update, it does suggest that you use a more accurate representation of Pi like 3.141592 when calculating wheel circumference. When used your distance measurements will now be more accurate. 

This version contains a new important My Block called **gyro turn to angle**. This block accurately turns your robot to a desired angle. The presentation now contains all the descriptions of this My Block, under the Gyro discussion, and shows all the math. 

The My Blocks called **gyro drive to waypoint** and **gyro drive by distance** now call **gyro turn to angle** first and then continue as before. For **gyro drive by distane** this means the distance is now very accurate as the turn is not using any of the distance at that point. The my block **gyro drive by time** does not first use **gyro turn to angle**. The reasons are all explained in the updated presentation. 

Finally all My Blocks that are for demo purposes have been udated with the word **demo** in the definition. 

To start a new project do the following...
1) Load up Spike Demo Final V2.llsp
2) Remove all the My Blocks that have the word demo in the definition.
3) Save the file to a new project name. 
Remember if you mess up the original you can always pull it from Github again. 
