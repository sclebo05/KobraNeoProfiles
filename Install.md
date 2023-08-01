# KobraNeoProfile Installation

### To add the profile to Cura:
- Ensure that you install **Cura 5.3.0 Beta** or newer.  It is possible to have more than one version of Cura installed.
- Create a new printer (Settings -> Printer -> Add Printer) and add an **Anycubic Kobra** if you do not already have one.
- With that printer selected in the main window, go to Preferences -> Configure Cura. 
- Within the Profiles section, use the Import button and select the desired .curaprofile file.  
- To switch between profiles in the main window, use the drop-down in the Print Settings dialog.
- Adjust your temperatures for better flow or to mitigate stringing. I have set reasonable PLA/PLA+ defaults
- Highly recommend adding the contents of the Cura-KobraNeoGCodes.txt file to the Machine Settings of the Kobra. 
  Settings -> Printers -> Manage Printers -> AnyCubic Kobra -> Machine Settings and paste the Start and End sections. Both of these sections are intended to REPLACE what is in there. Copying the existing code to a text file is not a terrible idea if you wish to revert later.

### To add the profile to Prusa or SuperSlicer:
- Go to File -> Import -> Import Config
- Select the desired config.ini file for import
- Once imported, go through Print Settings, Filament, and Printer sections and click the Save Icon to save/rename the profiles locally
- Highly recommend adding the contents of the Prusa-KobraNeoGcodes.txt file under the Custom G-code section of Printer Settings (Expert).  REPLACE what is in each section. Copying the existing code to a text file is not a terrible idea if you wish to revert later.

--- 

I've been working on these profiles in between my desired prints.  An occasional coffee helps me with the filament (and time) that I burn while testing. Throw a coffee my way, it's appreciated!

<a href="https://www.buymeacoffee.com/PYwIRuDB11" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
