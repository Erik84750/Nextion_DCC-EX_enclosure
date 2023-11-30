# Nextion_DCC-EX_enclosure
Files for 3D printing of DCC-EX_Nextion-controller enclosures

1. Introduction:
  This repository serves as a source for 3D printable enclosures for the Nextion DCC-EX project on this location: https://github.com/normhal?tab=repositories
  This repository contains the .stl files for 3.2", 3.5", 4.3" and 5" Nextion display enclosures

2. Features:
  a. the enclosure contain the necessary mounting tabs for a master-PCB and a 2x 18650 Li-Ion battery/charger/UPS.

  b. the encmosure provides the proper mounting points for the applicable Nextion display
  c. hoes are provided for an ON/OFF switch and a jack 3-pole receptacle for wired tethering (RX, TX, GND)
  d. an opening for USB-C charging connection
  e. openings for a rotary encoder and for 2 LED's (batteries charging and batteries charged).

4. Hardware requirements:
  a. the master pcb can be manufactured from the provided Gerber files. Beware of the mounting hole dimensions and psotions when making your own PCB)
  b. the battery holder and charging circuitry are contained on one PCB with specific mounting holes. Use this reference as a source: https://tinyurl.com/5b3ys9ak
    Make sure a 5V DC output version is used.
  c. the rotary encoder needs to be  the basic version (no pcb attached) due to space constraints
  d. the 2 front LED's are 3mm
  e. the external tethering jack 3.5mm receptacle needs to be this version as a reference: https://tinyurl.com/3r4jh7u7
  f. for mounting the lid, PCB and battery charger these brass M3 heat-inserts: M3 OD 4.2mm length 3mm, and M3 OD 5mm length 5mm:
    https://tinyurl.com/fwtkpy7e

5. 3D printing requirements:
  a. A minimal printing bed surface of 260x240mm is necessary (ie Anycubic Vyper)
  b. it is recommended to use a bimetal titanium throat: https://tinyurl.com/mrxmm24h
  c. only use high quality PLA filament: due to the complexity of the model (overhangs, holes, ..). For example: Prussa, Spectrum, ..
    Suboptimal results were obtained with Fiberlogy, eSun, and of course house brands or knock-offs which are off-limits.
  d. Some basic printer settings: Retraction = 9mm, Printing speed = 65mm/sec, no support structure, filling thickness 60% (2mm line distance),
    Filling pattern: cubic, Layer height 0.1mm, Wall thickness 0.8mm, Number of wall lines: 2, Print temp (Spectrum): 205°C, Bed temp: 60°C


     
