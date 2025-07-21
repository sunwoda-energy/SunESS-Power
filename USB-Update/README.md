# Updating the SunESS Power firmware using USB disk #
## 2025-07-11 ##

## Please preapre a USB disk (jump drive) in Fat32 or exFat format ##

#Step 1# 
  a) copy the .bin files to the USB disk root folder
  b) create “CmdConfig.txt” (case sensitive) in the root folder where the file contains:
  
update
1.SunEss_M3_App_ACea-0008_20250710.bin 
2.SunEss_PV_APP_ACda-0027_20250710.bin 
3.SunEss_PV_APP_ACda-0027__20250709.bin 

whereas “CmdConfig.txt” shall read in a text editor with shown symbol in square brackets: 
[line1]update[CRLF]
[line2]1.SunEss_M3_App_ACea-0008_20250710.bin[CRLF]
[line3]2.SunEss_PV_APP_ACda-0027_20250710.bin[CRLF] 
[line4]3.SunEss_PV_APP_ACda-0027__20250709.bin[CRLF] 


#Step 2#
  a) insert the USB disk into the debug port on the side of the inverter. 
  b) wait until all LED in the front of the SunESS power flashed quickly (every 0.5 second), roughly 10 mins (3 files). 
  c) remove the USB disk, and the system shall restart by itself. 

#Step 3# 
  The system shall generate automatically "DiskUpdatingInf.txt" on the USB disc which contains the serial number and the files used for the update, system component name (EMS/PCSAC/PCSDC) and update result (Update Success). 
  Please also use the mobile phone APP to check whether the software is up-to-date. 


  
