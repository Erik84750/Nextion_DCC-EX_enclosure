# Nextion_DCC-EX_enclosure
Files for 3D printing of DCC-EX_Nextion-controller enclosures

1. INTRODUCTION:

  This repository serves as a source for 3D printable enclosures for the Nextion DCC-EX project on this location: https://github.com/normhal?tab=repositories
  This repository contains the .stl files for 
  
  A. 3.2", 3.5", 4.3" and 5" Nextion display enclosures for custom-made pcb + charger/UPS unit with 2x 18650 Li-Ion batteries
  
  B. 3.2", 3.5" and 4.3" Nextion display enclosures for Wemos_ESP8266_18650 Li-Ion battery unit or Wemos_ESP32_18650 battery unit modules

  C. 3.5" and 4.3" Nextion display enclosures for Raspberry Pico are coming soon
  
        

2. FEATURES for version A

  a. the enclosure contain the necessary mounting tabs for a master-PCB and a 2x 18650 Li-Ion battery/charger/UPS.

  b. the enclosure provides the proper mounting points for the applicable Nextion display

  c. hoes are provided for an ON/OFF switch and a jack 3-pole receptacle for wired tethering (RX, TX, GND)

  d. an opening for USB-C charging connection

  e. openings for a rotary encoder and for 2 LED's (batteries charging and batteries charged).

  
  

3. HARDWARE REQUIREMENTS for version A:

  a. the master pcb can be manufactured from the provided Gerber files. Beware of the mounting hole dimensions and psotions when making your own PCB).
  See https://github.com/Erik84750/Nextion_DCC-EX_master-pcb
  
  b. the battery holder and charging circuitry are contained on one PCB with specific mounting holes. Use this reference as a source: https://tinyurl.com/5b3ys9ak
    Make sure the 5V DC output version is used. See picture below at bottom for modification instructions for this charger/UPS module.
    Marked "1": desolder the 2 SMD LED's and replace with wiring to the two 3mm LED's on the front panel; wiring is "common positive". 
    This means that the LED anodes both are connected together to the positive pad, and that the LED cathodes are sperarately connected each to their respective negative pad. 
    Marked "2": cut this LED.
    
  c. the rotary encoder needs to be  the basic version (no pcb attached) due to space constraints:
  
  ![rotary encoder wiring](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/b71eeac2-33ba-4ad2-aea9-3c3f7c741231)
  Wiring should preferably include a 10k pull-up resistor for OutA, OutB and Switch (D) and connected to +5V or +3V

  ![Rotary Encoder top view - basic wiring](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/7874d2f4-88f7-4a9a-8dbd-0af8db7db52f)

  
  d. the 2 front LED's are 3mm

  
  e. the external tethering jack 3.5mm receptacle needs to be this version as a reference: https://tinyurl.com/3r4jh7u7
  
  f. for mounting the lid, Nextion display, PCB and battery charger these brass M3 heat-inserts: M3 OD 4.2mm length 3mm, and M3 OD 5mm length 5mm:
    https://tinyurl.com/fwtkpy7e



4. 3D PRINTING REQUIREMENTS:

  a. A minimal printing bed surface of 260x240mm is necessary (ie Anycubic Vyper)
  
  b. it is recommended to use a bimetal titanium throat: https://tinyurl.com/mrxmm24h
  
  c. only use high quality PLA filament: due to the complexity of the model (overhangs, holes, ..). For example: Spectrum, to a lesser extent eSun..
    Suboptimal results were obtained with Fiberlogy, and of course house brands or knock-offs which are off-limits. Not recommended: Prussa, Azurefilm, Polymaker, Formfutura,..
    
  d. Some basic printer settings: Retraction = 9mm, Printing speed = 65mm/sec, no support structure, filling thickness 60% (2mm line distance),
    Filling pattern: cubic, Layer height 0.1mm, Wall thickness 0.8mm, Number of wall lines: 2, Print temp (Spectrum): 205°C, Bed temp: 60°C

  e. Some very good guides on Anycubic Vyper settings: https://tinyurl.com/2z6cprxj and https://tinyurl.com/yr662upk



![battery_charger_18560_UPS](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/30bb41c3-2cc0-40ef-bc59-00ba92e76630)


5. Hardware requirements for version B:

Either Wemos with ESP8266 with 18650 Li-Ion battery module or Wemos with ESP32 with 18650 Li-Ion battery unit.

Wemos_ESP8266 connections: rotary encoder: "Switch" to D1, "Clock" to D7, "Data" to D6. Others: Nextion TX to D2, RX to D5. Hardware RX and TX: as noted on the PCB.

Wemos_ESP32 connectiuons: self-explanatory on the PCB silkscreen. Rot. Enc. "Switch" to GPIO13, "Clk" to GPIO5, "Dat" to GPIO4. Nextion RX to GPIO3, TX GPIO17.



![Wemos_ESP8266](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/2a78477c-46e7-4568-a621-8d5ff625d159)


![Wemos_ESP32](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/cd38bd68-2209-46b7-a078-d1826cf59e98)


6. Hardware modifications on the module for version B:

  a. see picture below. Remove the 1-pole ON/OFF/ON switch and replace by enclosure mounted single pole double throw switch (BEWARE: only the left and center solderpads need to be connected to the switch)

  b. modify the pcb per picture: 1. remove switch and 2. remove both SMD LED's and wire 2x 3mm LED's for casing mounting; common positive to both LED's anode, each LED "-" solderpoint to the appropriate LED cathode

  c. Both the ESP8266 and ESP32 have a very similar component layout.



![Wemos_mod_v1](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/9fa37202-cf63-4627-877d-13471f64242b)


![IMG_20240212_102925](https://github.com/Erik84750/Nextion_DCC-EX_enclosure/assets/20128852/eb850c10-4ebc-4173-909d-61f7638bcddb)

