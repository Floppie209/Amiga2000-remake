# Amiga2000-remake

A recreation of the Amiga2000 motherboard using Sprint Layout

If you want to build this board please use the gerbers in Amiga2000rev6.2-XU1-PST518B.mod.zip. The only thing not applied are the two resistorpacks at U603 and U604. I will add them later.

I started with the complete removal of all components of an Amiga2000 rev 6.2 motherboard. I than removed all the print and 
the green layer so the bare copper showed.
The motherboard was than scanned at 600 dpi on both sides (saved as jpeg) which than could be loaded in Sprint Layout 6.0.

Set the dpi of the scanned images to 600dpi
Set the board width to 416.95 mm and the board height to 346.25 mm
Adjust the x and y offset to lineup the scannes with the .lay file

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

The board is now fully working.
I rest my case


