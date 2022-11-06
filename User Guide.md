## User Guide

This guide is meant as a simplified version of the firmware README, with information that is up-to-date and relevant to Rana Digital users.

The link to the Rana Digital firmware is here: https://github.com/rana-sylvatica/pico-rectangle-rana-digital

Note: currently the README in the firmware repo is unchanged from stock pico-rectangle, which is made for 20-button controllers that do not have the additional left-hand key that the Rana Digital adds.  The information on how to enter the various modes is correct, but the remapping instructions will not work because of the different number of buttons.  See the section below in this guide for how to remap the buttons on the Rana Digital.

### For Melee:

- #### PC (Slippi)

Plug the controller in using a USB-C to USB-A cable.  In Slippi Dolphin controller configuration, set port 1 to "GameCube Adapter for Wii U".  To ensure lowest possible latency, the Rana Digital emulates a GameCube Controller connected to a GCC adapter, eliminating the need for a physical adapter.

- #### Console

Plug the controller in using a GCC to USB-A cable.

### For Ultimate:

#### (Coming Soon)

### For Rivals of Aether:

#### (Coming Soon)

### Modes

This is not an exhaustive list of all the modes available in the pico-rectangle firmware but it should contain the ones that are useful to the vast majority of users.

#### (Coming Soon)

### Remapping

To enter remapping mode, hold down the highlighted key shown below when plugging in the controller.  Release the key within 3 seconds of plugging in.

![image](https://user-images.githubusercontent.com/95242582/200139452-89966a1b-7011-48a5-aa38-6df6dad52511.png)

After 3 seconds have passed, press the keys in the following order, corresponding to your preferred layout:

 - L
 - Left
 - Down 
 - Right
 - MX
 - MY
 - Start
 - CLeft
 - CDown
 - CUp
 - A
 - CRight
 - R
 - B
 - Y
 - X
 - LS
 - Z
 - MS
 - Up
 - DpadToggle/Up2 (depending on the mode)

Once all 21 keys have been pressed, unplug the controller and plug it in again.  If done correctly, it will now have your updated key mapping saved.  The mapping will not reset to default upon updating the firmware.

### Updating firmware

To update the firmware, first download the .uf2 file from: https://github.com/rana-sylvatica/pico-rectangle-rana-digital/releases

Then, plug in the controller to the PC while holding the highlighted key.  The controller will appear as a USB storage device.  Simply drag and drop or copy and paste the .uf2 file into this USB storage device.  The controller will disconnect and then reconnect in the default mode (emulated GCC adapter).

![image](https://user-images.githubusercontent.com/95242582/200201359-dd910422-d2cd-4318-995a-8f888dfb1723.png)

