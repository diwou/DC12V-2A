# DC12V-2A

![](https://codeberg.org/diwou/DC12V-2A/raw/branch/main/Images/DC12V-2A.jpg)

Please excuse the lousy picture. But unfortunately my ######## high-tech #### phone for over 1000 euros has such a ####### camera.... :-)



## DC converter for 12V in TO-3 format

This DC converter is the twin brother of [this 5V version](https://github.com/DL2DW/DC5V-2A) I had already uploaded here on GitHub recently. These serve among other things as a replacement for the Commodore 1541 floppy. On the one hand the current consumption decreases and as a consequence less power is converted into heat. This keeps the inside of the floppy drive much cooler.



## Technical

A switching regulator from Texas Instruments in the form of the TPS54332DDAR was used. On the one hand, this is exactly what I needed in terms of data, it is inexpensive and easy to install.

I designed the converter to handle 12V with a continuous load of 2A. 

The DC Converter can easily replace, for example, the well-known 7812 in TO-3 format, but still has enough reserve.

I once created a 3D image, because I unfortunately could not get sharp photos.

![](https://codeberg.org/diwou/DC12V-2A/raw/branch/main/Images/DC12V-2A_PCB_3D.jpg)



The 1541 draws up to 800mA under 12V, depending on the activity. The controller itself is designed for 2A, but can easily handle 3A for a short time. 

Under full load, that is 2A the ripple still looks pretty good in my opinion. I tested this with a resistive load (load resistors).

![](https://codeberg.org/diwou/DC12V-2A/raw/branch/main/Images/DC12V-2A_PCB_ripple.png)



## BOM

Here is the parts list for the DC converter. Of course you don't have to use exactly these brands. However, I give to note that comparison types, especially if they have a somewhat poorer quality, can have a negative effect on the ripple.

| Quantity | Designator | Manufacturer 1     | Manufacturer  Part Number 1 | Description                                                  |
| -------- | ---------- | ------------------ | --------------------------- | ------------------------------------------------------------ |
| 1        | C1         | Murata             | GRM155R71A104KA01D          | CAP  CER 0.1UF 10V X7R 0402                                  |
| 2        | C2,  C3    | TDK                | C3225X7R1H106M250AC         | TDK  - C3225X7R1H106M250AC - C3225X7R1H106MT000E             |
| 2        | C4,  C5    | TDK                | C3216X6S1V106K160AC         | Cap  Ceramic 10uF 35V X6S 10% SMD 1206 105°C Punched Paper T/R |
| 1        | C6         | Samsung            | CL21C100JBANNNC             | Cap  Ceramic 10pF 50VDC C0G 5% SMD 0805 Paper T/R            |
| 1        | C7         | Murata             | GRM033R71A822KA01D          | Multilayer  Ceramic Capacitors MLCC - SMD/SMT 0.0082uF 10volts 10% |
| 1        | C8         | KEMET              | C0805C202J3GACTU            | Multilayer  Ceramic Capacitors MLCC - SMD/SMT 25volts 2000pF C0G 5% |
| 2        | CN1,  CN2  | Mill-Max           | 3125-2-00-80-00-00-08-0     | CONN  PC PIN CIRC 0.040DIA TIN                               |
| 1        | D1         | MCC                | SS14FL-TP                   | DIODE  SCHOTTKY 40V 1A DO221AC                               |
| 1        | L1         | TDK  EPCOS         | B82464G4682M000             | Inductor  Power Shielded Wirewound 6.8uH 20% 100KHz Ferrite 4.3A 0.02Ohm DCR Automotive  T/R |
| 1        | R1         | Vishay             | CRCW0402169KFKED            | VISHAY  - CRCW0402169KFKED - RES, THICK FILM, 169K, 1%, 0.063W, 0402, REEL |
| 1        | R2         | Vishay             | CRCW040210K2FKED            | VISHAY     CRCW040210K2FKED.      Surface Mount Chip Resistor,  Thick Film, AEC-Q200 CRCW Series, 10.2 kohm, 63 mW, 1%, 50 V |
| 1        | R3         | Vishay             | CRCW040260K4FKED            | VISHAY  - CRCW040260K4FKED - SMD Chip Resistor, 0402 [1005 Metric], 60.4 kohm, CRCW  e3 Series, 50 V, Thick Film, 63 mW |
| 1        | R4         | Vishay             | CRCW040217K8FKED            | VISHAY  - CRCW040217K8FKED - RES, THICK FILM, 17K8, 1%, 0.063W, 0402 |
| 1        | R5         | Vishay             | CRCW0402732RFKED            | RES,  THICK FILM, 732R, 1%, 0.063W, 0402, REEL; Product Range:AEC-Q200 CRCW Series;  Resistance:732ohm; Power Rating:63mW; Resistance Tolerance: 1%; Voltage  Rating:50V; Resistor Case Style:0402 [1005 Metric]; Packaging:Tape & Reel  ;RoHS Compliant: Yes |
| 1        | U1         | Texas  Instruments | TPS54332DDAR                | TEXAS  INSTRUMENTS - TPS54332DDAR - DC/DC CONV, BUCK, 1MHZ, SOIC-8 |



# License

The contents of this repository, with the exception of the Docs and Software directories, are released under the following license:

- the "Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License" (CC BY-NC-SA 4.0) full text of this license is included in the [LICENSE.CC-NC-BY-SA-4.0](https://codeberg.org/diwou/DC12V-2A/raw/branch/main/LICENSE.CC-NC-BY-SA) file and a copy can also be found at https://creativecommons.org/licenses/by-nc-sa/4.0/
