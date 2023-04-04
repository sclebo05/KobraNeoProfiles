# KobraNeoProfiles

Had trouble finding Cura profiles for the Kobra Neo - most were derived from other printers, but none seemed to account for the bed leveling (M240 code) AND the direct drive.  Also wanted to stir in some of the Ender3 tweaks provided by CHEP's awesome Filament Friday channel https://www.youtube.com/@FilamentFriday

Created the Cura profiles for Cura 5.3.0 Beta found at https://github.com/Ultimaker/Cura/releases and used the Anycubic Kobra printer preset as a starting point.

**The KobraNeoGcodes.txt file has useful start and end codes for the printer, copy and paste these into your slicer's machine settings. I believe this was an important step, as it calls the auto leveling mesh information before beginning the print. Helps with any profile, not just these.**

### Key areas that were adjusted:
- Conservatively increased speeds (e.g. 50mm/s to 55mm/s)
- Increased the overlap values between infill and walls
- Reduced the number of walls and top/bottom layers
- Ensure that walls print before infill, reducing artifacts
- Adjusted flow rates
- Monotonic top, to make top surface more presentable
- Adjusted the Top/Bottom line direction - normally moves X and Y at 45 degrees, now moves X back and forth and increments Y row by row. (90,0)
- I primarily print in PLA+, so temps are a few degrees higher. Tune to taste.
- Disabled power-loss recovery to prevent blobbing and odd behavior during resume
- Up to 20% faster and with far less underextrusion issues and cleaner walls
- Added a 'fast' profile for even more speed, sacrificing accuracy

Added an example .jpg of a 3Dbenchy printed with original and new profiles [here](Original-and-new-Examples.jpg)

### To add the profile to Cura:
- Ensure that you install **Cura 5.3.0 Beta** or newer.  It is possible to have more than one version of Cura installed.
- Create a new printer (Settings -> Printer -> Add Printer) and add an **Anycubic Kobra** if you do not already have one.
- With that printer selected in the main window, go to Preferences -> Configure Cura. 
- Within the Profiles section, use the Import button and select the desired .curaprofile file.  
- To switch between profiles in the main window, use the drop-down in the Print Settings dialog.
- Adjust your temperatures for better flow or to mitigate stringing. I have set reasonable PLA/PLA+ defaults
- Highly recommend adding the contents of the KobraNeoGCodes.txt file to the Machine Settings of the Kobra

### To add the profile to Prusa or SuperSlicer:
- Go to File -> Import -> Import Config
- Select the desired config.ini file for import
- Once imported, go through Print Settings, Filament, and Printer sections and click the Save Icon to save/rename the profiles locally
- Highly recommend adding the contents of the KobraNeoGcodes.txt file under the Custom G-code section of Printer Settings (Expert)

### Firmware Upgrades:
I would advise against upgrading firmware AND playing with profiles until you have your printer reasonably tuned. Doing both at once could lead to some frustration.

Anycubic has firmware 1.2.8 available on their website. Many printers are shipping with a newer version. If you're interested in upgrading your printer's firmware, the official sources for 1.3.3 can be found at https://github.com/ANYCUBIC-3D/Kobra_Neo

Build intructions can be found at https://www.reddit.com/r/anycubic/comments/y2waxu/tutorial_how_to_build_anycubic_marlin_source_code/

A few github contributers have forked the original source code to provide other enhancements. Do so at your own risk. The above profiles are designed to work with 'stock' firmware from the vendor.

--- 

I've been working on these profiles in between my desired prints.  An occasional coffee helps me with the filament (and time) that I burn while testing. Throw a coffee my way, it's appreciated!

<a href="https://www.buymeacoffee.com/PYwIRuDB11" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
