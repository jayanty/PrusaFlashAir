# PrusaFlashAir
Applescript to sync a local folder with a Toshiba W-04 WiFi card

I followed these steps to setup a folder on my Mac that is kept in sync with a Toshiba W-04 WiFi SD card attached inside a Prusa Mk3 3D printer. Now each time I slice a new project, I save the output to my printer folder and the gcode file is automatically sync'ed with the SD card (If the printer is ON). Delete old files from this folder and they are also removed automatically from the SD card.

This will only sync gcode files to the SD card

Dependencies:
A lot of the backend heavy lifting is done using this codebase (https://github.com/CrashCash/FlashAirScripts) so you will need to install that first before following the steps below. Keep a record of where you put these scripts - that path will have to be updated in the Automator script later

Setup
1. Create a local folder that will be kept in sync with the SD card
2. Download the ZIP file to your computer and extract contents to a place where you want to save the script
3. Open Automator on the Mac and start a new project
4. Choose type as Folder Action for the document and click on Open an Existing Document
5. Navigate to where you extracted the contents of the ZIP file and select the package SyncToSD
6. Automator opens a window showing the project code: On top of this window you need to use the drop down to choose the folder you have designated as your local synced folder 
7. At the start of the script, customize the variables for your environment
8. Save the project and its ready to use
