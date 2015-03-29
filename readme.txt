/*
////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////
////////////////////	Known Issues	////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////

Please read these before reporting any bugs or issues to me.
						
-Health values are capped at 5 digits. This can be increased, but I wont because...
-Health values 32768 and above don't display the enemy health bar properly, but the numbers are still shown and are accurate.
-Enemy health bar does not show up if you are more than a certain distance away from the enemy (1024 map units).
-Resolutions below 640x480 are not supported.
-Using the console/menu to change the hud settings takes at least one in-game tic to change.


////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////
////////////////////	Adding HUD to your mod	////////////////////////////////
////////////////////////////////////////////////////////////////////////////////
////////////////////////////////////////////////////////////////////////////////

The following is for users who are already running another custom HUD.


Copy and paste the following files & directories into your mod:
acs
scripts (optional, but recommended if you want to modify anything)
graphics

loadacs
cvarinfo
menudef (optional)


If you intend to replace the graphics, here is a short guide to getting it to work:
-You will need at least 3 graphics: the border, the background, and the foreground
-Adjust your graphic offsets so that the background and foreground are within the border when displayed on top of each other
-Note the foreground's dimensions. If it is a horizontal bar, use the x value. If it is vertical, use the y value.
-In the acs script, modify the defines with your dimension, and the clipping offsets if necessary.
-If you need to replace the graphic names, search and replace these names in the script: HBARTOP, HBARBOT, HBARBRD

*/

