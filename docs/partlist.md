# Parts list

Everything needed for **one Cubeling cube**. All parts come from two EU shops, so no AliExpress and no customs.

> Prices checked in October 2026 and may have changed since. Buying for several cubes at once unlocks bulk prices and free shipping.

## Per cube

| # | Part | Qty | Shop | Price (each) | Notes |
|---|------|-----|------|--------------|-------|
| 1 | ESP32-C3 SuperMini Plus, soldered headers | 1 | [TinyTronics](https://www.tinytronics.nl/en/development-boards/microcontroller-boards/with-wi-fi/esp32-c3-supermini-plus-development-board-with-soldered-headers) | €5.00 | The brain. Wi-Fi/BLE, runs MicroPython |
| 2 | ESP32-C3 SuperMini Expansion Board | 1 | [TinyTronics](https://www.tinytronics.nl/en/development-boards/accessories/adapter-boards/esp32-c3-supermini-expansion-board) | €4.50 | Breaks out the pins and has a built-in LiPo charger |
| 3 | 0.96" OLED, 128×64, white, I2C (SSD1306) | 1 | [TinyTronics](https://www.tinytronics.nl/en/displays/oled/0.96-inch-oled-display-128*64-pixels-white-i2c) | €4.75 | The front screen. €4.50 at 10+ |
| 4 | MPU-6050 accelerometer + gyro | 1 | [TinyTronics](https://www.tinytronics.nl/shop/nl/sensoren/acceleratie-rotatie/mpu-6050-accelerometer-en-gyroscope-3-axis-module-3.3v-5v) | €8.75 | Tilt and shake detection, keeps the picture upright |
| 5 | Magnetic pogo connector pair, 2-pin, 90°, without eyelets | 4 | [BerryBase](https://www.berrybase.de/en/detail/0195a3b1f68970d39e2c9236d13477ec) | check shop | One pair per edge, split across faces (see ideas.md) |
| 6 | LiPo 3.7 V 500 mAh (LP-503035), JST plug | 1 | [BerryBase](https://www.berrybase.de/lp-503035-lithium-polymer-lipo-akku-3-7v-500mah-mit-2-pin-jst-stecker) | check shop | Has a protection circuit built in |
| 7 | 3D-printed shell | 1 | own printer | ~€1 filament | Needs slots that hold the connectors in exact positions |

**Estimated total: about €35–40 per cube.**

## Shared supplies (buy once)

- Thin hookup wire
- Solder + soldering iron
- A few M2 screws to mount the boards in the shell
- USB-C cable for programming and charging

## Before ordering

- [ ] Check that the expansion board's battery connector matches the JST plug on the LiPo. If not, cut and solder the leads.
- [ ] Check the connector dimensions on the BerryBase page: two need to fit side by side on each edge (~15 mm max each on a ~45 mm cube).
- [ ] BerryBase ships free from €150, so order several cubes' worth at once.
- [ ] Some TinyTronics items show 2–4 weeks delivery; check stock first.

## Why these parts

- **ESP32-C3 SuperMini** instead of an Adafruit QT Py: about €5 instead of €15, and still runs MicroPython.
- **Expansion board** gives battery charging without a separate TP4056 board, so less wiring.
- **2-pin connectors** are enough: each one carries ground + one signal line (plug = send, socket = receive).
- **Two shops only**: TinyTronics for the electronics, BerryBase for connectors and battery.
