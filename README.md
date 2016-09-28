# **Arduino IDE install files for duinoPRO**

**Installing the duinoPRO firmware environment:**

- Download and install the standard Arduino environment for your operating system. We have known support so far for OS X 10.11 and Windows 7 and 8.  The Arduino IDE download page is https://www.arduino.cc/en/Main/Software.  

**Note** that version 1.6.6 exhibits a known bug that effects duinoPRO.  We recommend downloading and installing 1.6.7.
 
- Start the Arduino IDE.
- From the menu, select *File | Preferences* in Windows or *Arduino | Preferences* on OS X.
- Add the following to *Additional Boards Manager URLs*: *https://raw.githubusercontent.com/duinoPRO/install/master/package_duinopro_index.json*.  Press ok.
- From the menu, select *Tools | Board “xx” | Boards Manager*.
- There should be an item *duinoPRO AVR Boards* (although it may take a little while to appear, while the json file is downloaded).  Select it and press the install button.  Wait while it installs.
- When you exit this menu and click on *Tools | Board “xx”* again, you should see *duinoPRO Uno* in the list of available boards.

**Installing the libraries:**
- Download the duinoPRO firmware repository as a zip file from https://github.com/duinoPRO/firmware.
- Unarchive.  You only require the libraries directory so you may discard the rest.
- Copy the contents of the libraries directory into: 
<br>*C:\Users\\\<yourusername>\Documents\Arduino\libraries* on Windows
or
<br>*/Users/\<yourusername>/Documents/Arduino/libraries* on OS X
- Restart the Arduino IDE. 
- The downloaded duinoPRO libraries should now appear under *Contributed libraries* when you click on *Sketch | Include Library*.  Click on them to include them in your sketch as per regular Arduino libraries. 
- Example libraries should now be available under *Examples from Custom Libraries* when you click on *File | Examples*.  Click on one to open it in a new window as per regular Arduino example sketches.

