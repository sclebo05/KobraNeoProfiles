# KobraNeoProfiles

Had trouble finding Cura profiles for the Kobra Neo - most were derived from other printers, but none seemed to account for the bed leveling (M240 code) AND the direct drive.  Also wanted to stir in some of the Ender3 tweaks provided by CHEP's awesome Filament Friday channel https://www.youtube.com/@FilamentFriday

Created the Cura profiles in Cura 5.3.0 Alpha found at https://github.com/Ultimaker/Cura/releases and used the Anycubic Kobra printer preset as a starting point.

**The KobraNeoGcodes.txt file has useful start and end codes for the printer, copy and paste these into your slicer's machine settings. I believe this was an important step, as it calls the auto leveling mesh information before beginning the print.**

### To add the profile:
- Create a new printer (Settings -> Printer -> Add Printer) and add a Anycubic Kobra if you do not already have one.
- With that printer selected in the main window, go to Preferences -> Configure Cura. 
- Within the Profiles section, use the Import button and select the desired curaprofile file.  
- To switch between profiles in the main window, use the drop-down in the Print Settings dialog.

### Key areas that were adjusted:
- conservatively turned up the speeds (e.g. 50mm/s to 55mm/s)
- Adjusted overlap values between infill and walls
- Reduced the number of walls and top/bottom layers
- adjusted flow rates
- Monotonic top, to make top surface more presentable
- I primarily print in PLA+, so temps are a few degrees higher. Tune to taste.
- Up to 20% faster and with far less underextrusion issues and cleaner walls

Added an example .jpg of a 3Dbenchy printed with original and new profiles