# Documentation #

* Concept: release package

Periodically, you freeze a set of documents and call them a release. You might make a zip file that contains all of your documents and then calculate and record its MD5 hash so that you can verify that the file hasn't been corrupted. In general, the software world is far more advanced in this area than the mechanical and the electrical.

## Mechanical ##

* Mechanical drawings, usually released in a format that is weakly read-only, like PDF.

## Electrical ##

* Schematics
* Gerber files for PCB fabrication

## Bill of materials ##

Here's an example of a basic bill of materials used for ordering parts for a run of beta prototypes.

Manufacturer | manufacturer part number | distributor | distributor part number | quantity | cost | extended cost | description
---|---|---|---|---|---|---|---
Kingston | SD4/4GB | Newegg | N82E16820134474 | 1 | 4.99 | 4.99 | SD card
XP Power | VFT80US05 | Digikey | 1470-2348-ND | 1 | 28.00 | 28.00 | 5 V, 12 A power supply
TDK-Lambda | ZPSA20-12 | Digikey | 285-1747-ND | 1 | 23.31 | 23.31 | 12 V, 1.8 A power supply for mic
TDK-Lambda | ZPSA20-9 | Digikey | 285-1746-ND | 1 | 23.31 | 23.31 | 9 V, 2.45 A power supply for Arduinos
Tyco/TE | 327043 | Digikey | A27425-ND | 8 | 0.42 | 3.36 | Spade terminals |  22-16 AWG for #6 stud
Cinch | 6-140 | Digikey | CBB106-ND | 1 | 2.46 | 2.46 | Barrier terminal block
Molex | 38002-1461 | Newark | 94F8420 | 4 | 0.2 | 0.8 | 9.53 mm jumpers for barrier terminal block
Molex | 8550104 | Newark | 54H5447 | 12 | 0.27 | 3.24 | Female crimp terminals for power supply connectors
Molex | 9503031 | Newark | 38C8766 | 3 | 0.2 | 0.6 | 0.156" pitch connector housing, 3 pos, for power supply
Tyco/TE | 1838275-2 | Digikey | A97644-ND | 1 | 11.27 | 11.27 | M12 4 pos waterproof connector, male
Brad/Woodhead | 804000D01M040 | McMaster | 6897K36 | 1 | 32.02 | 32.02 | M12 pigtail with 4 pin female connector
