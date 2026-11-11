# Onderdelenlijst

Alles wat je nodig hebt voor **één Cubeling-kubus**. Alle onderdelen komen van twee Europese webshops: geen AliExpress en geen douanekosten.

> Prijzen gecontroleerd in oktober 2026, ze kunnen intussen veranderd zijn. Bestel je voor meerdere kubussen tegelijk, dan krijg je volumekorting en gratis verzending.

## Per kubus

| # | Onderdeel | Aantal | Winkel | Prijs (per stuk) | Opmerkingen |
|---|-----------|--------|--------|------------------|-------------|
| 1 | ESP32-C3 SuperMini Plus, met gesoldeerde headers | 1 | [TinyTronics](https://www.tinytronics.nl/en/development-boards/microcontroller-boards/with-wi-fi/esp32-c3-supermini-plus-development-board-with-soldered-headers) | €5,00 | Het brein. Wifi/BLE, draait MicroPython |
| 2 | ESP32-C3 SuperMini Expansion Board | 1 | [TinyTronics](https://www.tinytronics.nl/en/development-boards/accessories/adapter-boards/esp32-c3-supermini-expansion-board) | €4,50 | Breekt de pinnen uit en heeft een ingebouwde LiPo-lader |
| 3 | 0,96" OLED, 128×64, wit, I2C (SSD1306) | 1 | [TinyTronics](https://www.tinytronics.nl/en/displays/oled/0.96-inch-oled-display-128*64-pixels-white-i2c) | €4,75 | Het scherm vooraan. €4,50 vanaf 10 stuks |
| 4 | MPU-6050 versnellingsmeter + gyroscoop | 1 | [TinyTronics](https://www.tinytronics.nl/shop/nl/sensoren/acceleratie-rotatie/mpu-6050-accelerometer-en-gyroscope-3-axis-module-3.3v-5v) | €8,75 | Detecteert kantelen en schudden, houdt het beeld rechtop |
| 5 | Magnetisch pogo-connectorpaar, 3-pins, 90°, zonder oogjes | 4 | [BerryBase](https://www.berrybase.de/en/detail/0195a3c33b5e72af9bf324023e17b04e) | zie winkel | Eén paar per rand, verdeeld over de zijden. Pinnen: GND, 5 V, data (zie Ideas.md) |
| 6 | LiPo 3,7 V 500 mAh (LP-503035), JST-stekker | 1 | [BerryBase](https://www.berrybase.de/lp-503035-lithium-polymer-lipo-akku-3-7v-500mah-mit-2-pin-jst-stecker) | zie winkel | Heeft een ingebouwde beveiligingsschakeling |
| 7 | Schottky-diode, 1N5817 of gelijkaardig | 2 | TinyTronics | ~€0,10–0,25 | Voor de gedeelde 5 V-laadlijn (zie Ideas.md) |
| 8 | Weerstand 1 kΩ | 4 | TinyTronics | enkele centen | Eén per TX-lijn van een rand (zie build-and-wiring.md) |
| 9 | 3D-geprinte behuizing | 1 | eigen printer | ~€1 filament | Heeft sleuven nodig die de connectoren op exact de juiste plek houden |

**Geschatte totaalprijs: ongeveer €37–43 per kubus.**

## Gedeeld materiaal (één keer kopen)

- Dunne aansluitdraad
- Soldeertin + soldeerbout
- Een paar M2-schroefjes om de printplaten in de behuizing te monteren
- USB-C-kabel om te programmeren en op te laden

## Voor je bestelt

- [ ] Controleer of de batterijaansluiting van het expansion board past op de JST-stekker van de LiPo. Zo niet, knip de draden door en soldeer ze vast.
- [ ] Controleer de afmetingen van de connectoren op de BerryBase-pagina: er moeten twee 3-pins connectoren naast elkaar op elke rand passen (max. ~15 mm elk op een kubus van ~45 mm).
- [ ] BerryBase verzendt gratis vanaf €150, bestel dus voor meerdere kubussen tegelijk.
- [ ] Sommige TinyTronics-artikelen hebben 2–4 weken levertijd, controleer eerst de voorraad.

## Waarom deze onderdelen

- **ESP32-C3 SuperMini** in plaats van een Adafruit QT Py: ongeveer €5 in plaats van €15, en draait nog steeds MicroPython.
- **Expansion board** zorgt voor het opladen van de batterij zonder apart TP4056-bordje, dus minder bedrading.
- **3-pins connectoren**: massa, een gedeelde 5 V-lijn en één datalijn (stekker = zenden, contrastekker = ontvangen). Dankzij de 5 V-lijn laadt een hele rij kubussen op via één USB-kabel.
- **Diodes** voorkomen dat stroom de verkeerde kant op loopt tussen kubussen.
- **Maar twee winkels**: TinyTronics voor de elektronica, BerryBase voor de connectoren en de batterij.
