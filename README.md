# gimp_mib2std_boot_mage_save
Plugin for GIMP to open/save image for VW MIB STD2 PQ/ZR Technisat/Preh boot animation

NOTICE:
boot animation -is a series of 800x480 png images and separate labels (depending on the model / configuration) 480x100.
The base file format is png, but with the original color encoding. This project is an attempt to convert a mib png to a regular color image and back
All transformations have been obtained empirically and are certainly different from those in the system. 
Colors and shades may differ from those specified.


To install just extract to plug-ins folder of GIMP (in my case it's c:\Program Files\GIMP 2\lib\gimp\2.0\plug-ins) and restart GIMP

How to use:
create image with resolution 800x480 or 480x100 for label

In menu - select File\Export As... (Shift+Ctrl+E)
Set name\folder to export
In "Select File Type (By Extension)" (bottom left) choose "MIB2STD BOOT Image"

And press Export
system will prompt you to set color limit ...
it was found that a file larger than 1 MB is not installed in my system, so I have to limit the color
Default - 128, I used 64

...and will offer to extract label in separate file
if selected "Yes" and picture is 800x480
Result: 2 files
1 - Main picture (800x480) with an empty window for animated label (for size reduce) - "selected file name".mib
2 - Label picture (480x100) - "selected file name"_lbl.mib

Else
Result: 1 file
1 - Main picture (800x480) - "selected file name".mib

