# DC12V-2A

![](https://codeberg.org/diwou/DC12V-2A/raw/branch/main/Images/DC12V-2A.jpg)

Bitte entschuldigt das schlechte Bild. Aber leider hat mein ######## Hightech-####-Handy für über 1000 Euro eine ######## Kamera... :-)

---

## DC-Wandler für 12 V im TO-3-Format

Dieser DC-Wandler ist der Zwillingsbruder der [5V-Version](https://github.com/DL2DW/DC5V-2A), die ich vor Kurzem hier auf GitHub hochgeladen habe.

Er dient unter anderem als Ersatz für Spannungsregler in der Commodore 1541 Floppy. Zum einen sinkt der Stromverbrauch deutlich, wodurch weniger Leistung in Wärme umgewandelt wird. Dadurch bleibt das Innere des Laufwerks wesentlich kühler.

---

## Technische Details

Zum Einsatz kommt ein Schaltregler von Texas Instruments vom Typ **TPS54332DDAR**. Dieser erfüllt alle Anforderungen, ist günstig und leicht zu verbauen.

Der Wandler ist für eine **Dauerlast von 2 A bei 12 V** ausgelegt.

Er eignet sich hervorragend als Ersatz für klassische lineare Spannungsregler wie **7812**, mit dem Vorteil deutlich geringerer Wärmeentwicklung.

---

## Hinweise zum Einbau

Der Kühlkörper bzw. die Montagefläche sollte bei höheren Strömen für Wärmeabfuhr sorgen.  
Bei Verwendung in Geräten wie der 1541 reicht oft die passive Kühlung über das Gehäuse.

---

## Stückliste (BOM)

| Bezeichnung | Wert / Typ         | Beschreibung                                |
|-------------|---------------------|---------------------------------------------|
| IC1         | TPS54332DDAR        | Step-Down-Schaltregler von Texas Instruments |
| C1          | 10 µF / 25 V         | Eingangskondensator, Keramik                 |
| C2          | 47 µF / 25 V         | Ausgangskondensator, Low ESR                |
| L1          | 10 µH                | Induktivität, ≥ 2 A belastbar                |
| D1          | Schottky-Diode      | z. B. SS34 oder vergleichbar                 |
| R1, R2      | Spannungsteiler     | zur Einstellung der Ausgangsspannung        |
| Cff         | optional             | 100 pF zur Optimierung der Regelung          |
| Layout      | TO-3-kompatibel     | Passend für TO-3-Ersatz                      |

---

## Lizenz

Der Inhalt dieses Repositories steht unter folgender Lizenz:

**Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**  
Der vollständige Lizenztext befindet sich in der Datei [LICENSE.CC-NC-BY-SA-4.0](https://codeberg.org/diwou/DC12V-2A/raw/branch/main/LICENSE.CC-NC-BY-SA)  
Und ist auch online verfügbar unter: https://creativecommons.org/licenses/by-nc-sa/4.0/
