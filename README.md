# KobraNeoProfiles

Had trouble finding Cura profiles for the Kobra Neo - most were derived from other printers, but none seemed to account for the bed leveling (M240 code) AND the direct drive.  Also wanted to stir in some of the Ender3 tweaks provided by CHEP's awesome Filament Friday channel https://www.youtube.com/@FilamentFriday

Created the Cura profiles in Cura 5.3.0 Alpha https://github.com/Ultimaker/Cura/releases and used the Anycubic Kobra printer preset as a starting point.

The KobraNeoGcodes file has useful start and end codes for the printer, copy and paste these into your slicer's machine settings. I believe this was an important step, as it called the auto leveling mesh information.

To add the profile, create a new printer (Settings -> Printer -> Add Printer) and add a Anycubic Kobra if you do not already have one. With that printer selected in the main window, go to Preferences -> Configure Cura.  Within the Profiles section, use the Import button.  To switch between profiles in the main window, use the drop-down in the Print Settings dialog.

