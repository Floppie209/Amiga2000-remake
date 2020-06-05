# Amiga2000-remake

A recreation of the Amiga2000 motherboard using Sprint Layout

If you want to build this board please use the gerbers in Amiga2000rev6.2.incl.mods.1.8.5.zip. The only thing not applied are footprints for the r2-c1 combo as it involves moving a lot of traces and I dont know what it does to the working of the board. All other 6.2 fixes are applied.

I used the following data to order the pcbS at JLCPCB:
Layers - 2
PCB Dimension - 416.95mm * 346.25mm
PCB Qty - 5
PCB Thickness - 1.6mm
PCB Color - Blue
Surface Finish - ENIG-RoHS
Copper Weight - 2oz
Gold Fingers - No
Material Details - FR4-Standard Tg 130-140C
Panel by JLCPCB - No
Flying Probe Test - Fully Test
Castelated Holes - No
Different Design - 1
Remove Order Number - No

On their site you can check their capabilities but my board confirms to their minimum requirements.

I started with the complete removal of all components of an Amiga2000 rev 6.2 motherboard. I than removed all the print and 
the green layer so the bare copper showed.
The motherboard was than scanned at 600 dpi on both sides (saved as jpeg) which than could be loaded in Sprint Layout 6.0.

Set the dpi of the scanned images to 600dpi
Set the board width to 416.95 mm and the board height to 346.25 mm
Adjust the x and y offset to lineup the scannes with the .lay file

DO NOT POPULATE: C902, C917, R901, FB904, FB906, RP904, RP906, RP905, C230, C240, they are unpopulated on factory 6.2 rev, so, let them as-is.

In Sprint Layout I than placed all the components (the ones that weren't there I created myself).
Then I put in all the via's.

I am now busy with tracing all the connections with the scans as background.

Update 31-5-2019: 

Frontside finished. When the solderside is finished I will check both sides completely before sending the files of for fabrication.

Update 6-6-2019:

Solderside finished.
I checked both sides in close up. (took all day). I found a view missing ground connections and i think it is okay.

Update 7-6-2019:

Check started

Update 8-6-2019:

Check completed and fixed a view ground connections on the solderside. Also fixed up some polygons.
DRC issues fixed only silscreen on pad issues remain. I will leave those in as it is no problem for fabrication.
Uploaded the latest sprint-layout file and the gerberfiles.
Also I uploaded a jpeg of the finished board.

Update 14-6-2019:

Redone the powerconnector as on the test print the connector did not fit correctly.
As of that the board is now set to rev 1.1.
Uploaded the last sprint layout file and a zip file with the latest gerber files.

I will now send the gerber files for fabrication.
When the pcb comes back I will start soldering.

Update 17-6-2019:

Uploaded a new sprint layout file where some silkscreen partnumbers have been changed.

I strongly advice people to not make boards with these files for now.
I will do a test batch and completely solder a board for testing. If it checkes out I will let it be known here.

If people want to check it also be my guest but keep me informed if you find anything. (preferably with a screenshot).

Update 6-7-2019:

Boards arrived from the Fab. I tested the board for shorts between GND and the various powerlines and found no shorts.
I no started to solder the passive components to the board.
As I checked the silkscreen I found three typing mistakes which I rectified and therefore I updated the sprint files today.
I also made new gerberfiles which are in the corresponding zip file.

Update 20-7-2019:

Fixed a missing trace as the zorro slots were not functioning.
Board is functioning, the only problem left is the video expansion port not stable enough.

Update 8-8-2019:
Removed all versions of the old files and uploaded the final design, incl gerbers.
In this version almost all the 6.2 patches are applied.

Update 9-8-2019:
The problem with the videoextention slot is solved. Flickerfixers that use that slot are working fine now.
I made new gerbers and updated the github page.

Update 20-8-2019:
Changed some footprints and cleaned up the pcb a little.
New gerbers are uploaded

Update 27-8-2019:
I was pointed out that on the original board D15 of the isa slots was not terminated properly. On the original board this is the case. It is fixed in version 1.6 of the board. If you are not using the isa slots than version 1.5 works fine. Anyway I uploaded a 1.6 version of the board together with the gerber files.

Update 28-9-2019
Widened the +5V, +12V and -12V traces to 1.4 mm. If you populate all the slots it might not have enough power when trace is 1 mm. When you order the board with 70um copper it can now handle 6 amps. I uploaded a 1.7 version of the design and with it the gerber zip

Update 21-10-2019
Changed the battery to a buttoncell battery and placed an diode D803 as the buttonbattery cannot be charged. I also uploaded the bomfile created from the sprintlayout file for Rev 1.7.5.
Changed the Rev to 1.7.5 and uploaded new sprint and gerber files.

Update 7-11-2019
Widened the +5V and +12V traces to 1.6 mm. I uploaded new gerber files, sprint file and BOM file 1.8.
I also changed the rev number to Rev 1.8.

Update 10-11-2019
Added some SMD leds with resistors to show if some voltages are okay, also I widened the -12V traces to 1.6 mm. I changed the rev number to Rev 1.8.5 and uploaded new gerber files, sprint and BOM file.

Update 17-11-2019
John Hertell made a locator for version 1.8.5 of my Amiga2000 board. It can be found on:
http://locator.reamiga.info/locator.php?project=A2000.

Update 28-12-2019
I have finished the build of my 1.8.5 pcb. It started at the first try. I will not do any more updates on this page. If someone will build it he/she/it can use the gerber files and order one at a pcb factory.
I am happy with the result and say cherio.

Update 7-1-2020
I have put the order details in this readme file.

Update 5-6-2020
Changed the value of rp101 from 4.7k to 2.7k as thats the value in the schematic.
Also i added a list with ordernrs for several companies


