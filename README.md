# tips
repo  for some tips 
# Fix usb flash cards and CD cards

Make sure you have GParted installed. In a terminal window, run

`sudo apt install gparted`
Then open GParted as root (still in the terminal window):

`sudo gparted`
Select your USB stick from the GParted > Devices dropdown menu. Then click the "Device" tab > Create Partition Table...

This will erase all the data from the stick, so be sure you don't have anything valuable in it.

There will be an unallocated space left, double click it to create a new partition with your settings, such as disk label and filesystem (you'll probably want it to be NTFS).

Don't forget to apply your configuration by clicking the green "check" button in GParted.
