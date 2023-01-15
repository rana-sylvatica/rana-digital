# How to assemble a Rana Digital

These are the instructions for building the controller.  For information on ordering the parts please refer to the ordering guide.

## Step 1: Tools

Required:
 - Soldering iron
 - Solder
 - Flush cutters
 - 2mm hex key

Nice to have:
 - Isopropyl alchohol
 
## Step 2: Parts

Shell
 - 1x Rana Digital Chassis \*
 - 14x M3 x 5mm + 4mm Male to Female Hex Standoffs \*
 - 14x M3 x 4mm Button Head Hex Drive Screw
 - 1x Port Insert \*
 - 1x Backplate
 - 1x Foam Pad
 - Cyanoacrylate (superglue)
 - (OPTIONAL BUT RECOMMENDED) Purple Loctite threadlocker (low-strength, removable)

PCBs
 - 1x Rana Digital Mainboard
 - 1x RLUB (USB C breakout board)
 - 21x Kailh hotswap socket
 - 1x 8-pin 2.54mm pitch right angle male pin header
 - 1x 8-pin 2.54mm pitch right angle female pin header

Switches
 - 21x MX-style mechanical (not optical) keyboard switches
 - 21x circular keycaps
 - (OPTIONAL) 21x 0.5mm keyboard switch foam pads

\* - if you are using the segmented FDM printable version of the case, see the section at the bottom of this page for alternate parts for those marked with an asterisk. 

## Step 3: Flashing Firmware and Soldering

Since the Rana Digital Mainboard has the RP2040 MCU built-in there is no difficult soldering required for this build.

Prior to beginning soldering, plug the mainboard into a PC using the onboard USB C port.  If the board is functional it will appear as a USB storage device labeled "RPI-RP2". If this does not come up, the board is defective in some way.  Likely causes are that either the USB port or the RP2040 were assembled incorrectly at the factory. Errors like this are rare but can happen.

At this point if the board is functional, it is time to flash the firmware. Download the .uf2 file from the firmware page and copy and paste it into this storage device. It will disconnect from the PC which indicates successful flashing.

Unplug the board and turn it over so the SMD components are facing down and the "Rana Digital PCB" silkscreen is facing up.  Place the hotswap sockets into the board as shown, making sure that they sit flush against the board.

![IMG_20230107_130921577](https://user-images.githubusercontent.com/95242582/212520852-414e3f4f-d843-4749-8e12-c27db4e9310b.jpg)

Using the soldering iron, apply solder at the connection between the pad on the board and the pin on the hotswap socket.  The solder should flow and adhere strongly to both surfaces.  If it balls up or does not appear to stick properly, continue to apply heat and add a bit more solder.  When all 21 sockets have been soldered the board should look like this:

![IMG_20230107_152151010](https://user-images.githubusercontent.com/95242582/212520911-ff3ecb2e-4531-4961-a895-dd76ba009175.jpg)

Next it is time to solder the female pin header to the mainboard and the male pin header to the USB C breakout board.  If you ordered these from the link in the ordering guide they will come in 40-pin rows. Using flush cutters, cut an 8-pin section of each.

Next, solder the male pin headers on the USB C breakout board.  They generally come in a 40-pin row so you will need to cut an 8-pin section as shown.

![IMG_20230107_152247444](https://user-images.githubusercontent.com/95242582/212521261-dbcd13e4-b672-4145-9050-6d30af130793.jpg)

![IMG_20230107_152317256](https://user-images.githubusercontent.com/95242582/212521265-0460f7c0-8696-42ae-a055-adc99ce215b7.jpg)

To solder, turn the board over so the pins are sticking through from the bottom and the blank side (without pin labels) side of the board is facing up.  This orientation is very important.

![IMG_20230107_152317256](https://user-images.githubusercontent.com/95242582/212521509-dcdbf050-997e-47ef-b957-0522e087cdd5.jpg)

Apply solder to the connection between the sticking up pins and the pads on the board, making sure not to bridge adjacent pins.  It should look like this when finished:

![IMG_20230107_152546482](https://user-images.githubusercontent.com/95242582/212521542-875bd2c5-71d1-4ea7-af29-7b2a916aa1b0.jpg)

Next, solder the matching female pin header to the mainboard: Cut an 8-pin section, place it on the side of the board with the SMD components, and then turn the board over so the pins are sticking through from the bottom.  Use a flush cutter to trim the pins sticking out.  They don't need to be completely flush but no more than 1mm sticking up is ideal.  The trimming can be done either before or after soldering the pins, but if trimming after soldering make sure to reflow each soldered connection once finished with trimming.

![IMG_20230107_183231782](https://user-images.githubusercontent.com/95242582/212521721-82d28c14-0e14-4c96-9c52-5e965135db0c.jpg)
![IMG_20230107_183257611](https://user-images.githubusercontent.com/95242582/212521726-93387532-0170-4d41-927f-dffcd6eb32e3.jpg)
![IMG_20230107_183358145](https://user-images.githubusercontent.com/95242582/212521730-f8463a00-d123-48d6-b903-63b749c60dfc.jpg)
![IMG_20230107_183802299](https://user-images.githubusercontent.com/95242582/212521732-84c34302-9fff-4310-98fa-524ea2668d52.jpg)

At this point the soldering is complete.  It is recommended to clean the solder joints using isopropyl alchohol and either paper towel or an old toothbrush to remove flux residue.

(OPTIONAL) - to improve the sound profile of the controller a little bit you can use keyboard switch foam pads as shown. These are 0.5mm thick and just add a tiny bit of padding between the switch and the PCB.

![IMG_20230107_192443190](https://user-images.githubusercontent.com/95242582/212521913-b91d95c2-9f53-4144-92ab-f64c4063cd26.jpg)

## Step 4: Prepare the Chassis

Place a small drop of cyanoacrylate adhesive in each of the 14 hexagonal holes in the underside of the chassis.  Press a threaded standoff into each hole, making sure that it sits flush against the surface of the post.  Wipe off any excess glue with a paper towel.  Set aside to cure for an hour before final assembly (this isn't absolutely necessary but reduces the risk of accidentally pulling out a standoff with uncured glue).

![IMG_20230107_200422852](https://user-images.githubusercontent.com/95242582/212522009-a303f3f3-9d70-4656-88cb-9bef2dea7a97.jpg)

## Step 5: Assembly

Break off a Port Insert from the 6x sprue and put it in the gap in the chassis as shown so the holes line up with the threaded inserts below.

![IMG_20230107_200512509](https://user-images.githubusercontent.com/95242582/212544352-b2358ecb-1f5f-48c5-bf0b-304bda9b8686.jpg)
![IMG_20230107_200743212](https://user-images.githubusercontent.com/95242582/212544370-3060b53a-558e-4806-a653-8f9269bb870c.jpg)

Put the mainboard and USB C board in the chassis as shown.  The male pin header on the USB C board should be inserted into the female pin header on the mainboard and the USB C port should be inserted through the hole in the Port Insert component.  Use 6x of the 4mm M3 screws to attach the two boards to the chassis.  It is recommended but not required to use a small amount of low-strengh (purple) loctite threadlocker on these screws.

![IMG_20230107_201125959](https://user-images.githubusercontent.com/95242582/212544398-6f140bf5-e7e8-4a8a-a3a2-1310ceb35c3a.jpg)

Turn the controller over and insert the switches while supporting the PCB from the other side.  Make sure the pins on the switchs are not bent when inserting. The switch should clip into the square hole on the chassis and feel secure.

![IMG_20230107_201331715](https://user-images.githubusercontent.com/95242582/212544681-5cbca39e-0cac-444c-9679-ee9f312e9ec8.jpg)

When all the switches are properly inserted it should look like this:

![IMG_20230107_204143402](https://user-images.githubusercontent.com/95242582/212544685-19187bb1-c96b-44d8-88c1-d1badd678ae5.jpg)

At this point it is recommended to test the controller to make sure everything is working properly. If using the default Rana Digital firmware, hold Start (middle button) when plugging in to a PC to put it into keyboard mode. Open notepad or a similar program and press the buttons on the controller.  If it is working, each button should type a letter when pressed.  If a button does not, use a switch puller tool to pull the switch out of the board and check if one of the pins was bent during assembly.  If this did not seem to be the issue then look at the solder joints for that switch and reflow/add solder as needed.  At this stage it is also good t check GCC functionality.  Using the USB-GCC cable, plug the controller in to either a Wii/GameCube or a GameCube controller adapter and make sure the buttons function.

Once you have verified that the controller is fully functional, put on the backplate and the foam pad.  Simply screw in the 8 remaining 4mm M3 screws.  Again, it is recommended to use threadlocker to prevent the screws from working loose.  For the foam pad, just peel off the paper backing and stick onto the backplate.

![IMG_20230107_205454881](https://user-images.githubusercontent.com/95242582/212545131-14ae064c-d7e8-4b09-8261-8ef2d9473c46.jpg)

Finally, install the keycaps.  Break them off from the sprue and press on to each switch, making sure to match the orientation of the stem.  They can be somewhat tight so you will need to press firmly.

Once the keycaps are installed the controller is complete.  Enjoy!

![image](https://user-images.githubusercontent.com/95242582/212545908-9791519c-d152-4f1a-98bb-77aeb9e6b382.png)
![image](https://user-images.githubusercontent.com/95242582/212545916-333549ee-e8ed-427b-9d3b-0e1b23ca870b.png)


# Alternate Instructions for FDM Chassis:

If you are 3D printing the chassis using the split design intended for FDM printers, follow these instructions (from @davyiskewl#5038 on Discord who designed these modifications to the chassis).  Soldering and installing the PCBs, switches, backplate, and keycaps will all be the same as described above.

## Parts:

Instead of the male-to-female hex standoffs from the parts list at the top of this page you will need 18x M3 heat-set threaded inserts such as:

https://cnckitchen.store/products/gewindeeinsatz-threaded-insert-m3-standard-100-stk-pcs

or

https://www.amazon.com/AIEX-Printing-Embedment-Automotive-4-6x5-7mm/dp/B09TNK8GD6/

You will also need 18x of the 4mm M3 screws from the parts list at the top of the page.

## Print Files:

Use the files from the folder labeled FDM.  You will need to print a left half, a right half, and a port insert.

## Print Settings:

Printing the Rana Digital is fairly straightforward. See below for example settings (other settings may work as well, depending on your printer.  Settings also may vary based on your slicer software). Make sure to apply supports over the intersection of the start button as pictured. Nowhere else on the enclosure do you need supports.

![image](https://user-images.githubusercontent.com/95242582/212546527-50a6ac40-bbcf-45d9-bfcb-b68c6766424c.png)

I found that printing with a top layer produced weird artifacts as pictured. Printing without the top layer decreases print times and results in a cleaner print for me.

![image](https://user-images.githubusercontent.com/95242582/212546556-66ee4f3d-cf9b-4df0-a444-0de83ff283e3.png)
![image](https://user-images.githubusercontent.com/95242582/212546569-661182c6-de40-4f62-bf72-fe23cb67745b.png)

The resulting slice should look something like the following:

![image](https://user-images.githubusercontent.com/95242582/212546601-3c52c0ef-fbde-4f27-83bd-b1411a199d19.png)

Use the same setting for the other side.

Normal settings should suffice for printing the usbc port insert. No need for supports.
![image](https://user-images.githubusercontent.com/95242582/212546618-a9a4dcee-cd6b-41a3-8f34-9f88f182678a.png)

## Assembly

To assemble the case you will need a soldering iron (or some other way to press in the heated inserts), heat-set inserts, and M3 screws.

First start by placing heated inserts into their holes. The Right side has 7 + 4 (for the connection) and the Left side has 7.

![image](https://user-images.githubusercontent.com/95242582/212546721-b48e19ae-0112-431c-87be-7d0b637441ef.png)

Use your soldering iron to push the inserts into place. A little below flush is ok.

![image](https://user-images.githubusercontent.com/95242582/212546736-0dd944a7-293b-4771-9bac-d18548712b76.png)

Assemble the 2 halves of the case together as shown, by screwing in the 4 connecting screws.

![image](https://user-images.githubusercontent.com/95242582/212546813-097ecbe3-7be0-4835-8ede-9fd64a7c7b4a.png)

Finish pushing in the rest of the heated inserts in if you haven’t already. That’s it! You’re done! You now have a completed 3d printed Rana Digital enclosure. Return to the rest of the instructions for finishing the controller.

![image](https://user-images.githubusercontent.com/95242582/212546866-631fd023-beaf-4729-88aa-16b0d058aa3c.png)

![image](https://user-images.githubusercontent.com/95242582/212546875-5ce15f99-6807-4605-a244-952e055eae72.png)

