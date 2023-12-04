# Nextion_DCC-EX_enclosure
Files for 3D printing of DCC-EX_Nextion-controller enclosures

1. INTRODUCTION:

  This repository serves as a source for 3D printable enclosures for the Nextion DCC-EX project on this location: https://github.com/normhal?tab=repositories
  This repository contains the .stl files for 3.2", 3.5", 4.3" and 5" Nextion display enclosures


2. FEATURES:

  a. the enclosure contain the necessary mounting tabs for a master-PCB and a 2x 18650 Li-Ion battery/charger/UPS.

  b. the enclosure provides the proper mounting points for the applicable Nextion display

  c. hoes are provided for an ON/OFF switch and a jack 3-pole receptacle for wired tethering (RX, TX, GND)

  d. an opening for USB-C charging connection

  e. openings for a rotary encoder and for 2 LED's (batteries charging and batteries charged).



3. HARDWARE REQUIREMENTS:

  a. the master pcb can be manufactured from the provided Gerber files. Beware of the mounting hole dimensions and psotions when making your own PCB).
  See https://github.com/Erik84750/Nextion_DCC-EX_master-pcb
  
  b. the battery holder and charging circuitry are contained on one PCB with specific mounting holes. Use this reference as a source: https://tinyurl.com/5b3ys9ak
    Make sure a 5V DC output version is used. See picture below for modification instructions for this charger/UPS module.
    Part 1: desolder the 2 SMD LED's and replace with wiring to the two 3mm LED's on the front panel; wiring is "common positive". 
    This means that the LED anodes both are connected together to the positive pad, and that the LED cathodes are sperarately connected each to their respective negative pad. 
    Part 2: cut this LED.
    
  c. the rotary encoder needs to be  the basic version (no pcb attached) due to space constraints
  
  d. the 2 front LED's are 3mm
  
  e. the external tethering jack 3.5mm receptacle needs to be this version as a reference: https://tinyurl.com/3r4jh7u7
  
  f. for mounting the lid, Nextion display, PCB and battery charger these brass M3 heat-inserts: M3 OD 4.2mm length 3mm, and M3 OD 5mm length 5mm:
    https://tinyurl.com/fwtkpy7e



4. 3D PRINTING REQUIREMENTS:

  a. A minimal printing bed surface of 260x240mm is necessary (ie Anycubic Vyper)
  
  b. it is recommended to use a bimetal titanium throat: https://tinyurl.com/mrxmm24h
  
  c. only use high quality PLA filament: due to the complexity of the model (overhangs, holes, ..). For example: Prussa, Spectrum, ..
    Suboptimal results were obtained with Fiberlogy, eSun, and of course house brands or knock-offs which are off-limits.
    
  d. Some basic printer settings: Retraction = 9mm, Printing speed = 65mm/sec, no support structure, filling thickness 60% (2mm line distance),
    Filling pattern: cubic, Layer height 0.1mm, Wall thickness 0.8mm, Number of wall lines: 2, Print temp (Spectrum): 205°C, Bed temp: 60°C

  e. Some very good guides on Anycubic Vyper settings: https://tinyurl.com/2z6cprxj and https://tinyurl.com/yr662upk



![battery_charger_18560_UPS](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/30bb41c3-2cc0-40ef-bc59-00ba92e76630)

    


     
