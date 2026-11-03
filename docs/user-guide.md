# User guide (draft)

## In the box

- Radar board with its antenna: lens radome (20 m kit) or horn antenna with PTFE lens (60 m kit)
- USB-to-TTL serial adapter (CH340) with Dupont jumper wires
- Download access: this repository (GUI, protocol notes, user guide, datasheets)

## Wiring (UART)

Set the adapter's voltage jumper to **3.3 V**. Cross the data lines:

| Adapter | Radar board |
|---|---|
| TXD | RX0 |
| RXD | TX0 |
| GND | GND |

Pin names are printed on the board. On the 60 m board, TX0 and RX0 are pins 1 and 2 of the H1 header
(2 × 8, 2.0 mm pitch).

## Power

- 20 m board: 3.3 V on 3V3 (3.1–3.5 V), 135 mA typical, 600 mA max. Use a supply rated 1 A or more with
  ripple below 50 mV.
- 60 m board: power is on the H2 header (5V_IN, 5V_EN, GND). Step-by-step wiring with photos will be
  added here.

## First measurement

1. Mount the antenna facing the surface to be measured, as close to the vessel centre as possible.
2. Start `RadarGUI.exe`, choose the adapter's COM port, 115200 baud.
3. Read the distance. Set the range, blind zone and offset for your vessel, then run false-echo learning
   with the vessel empty or at a known level.

Screenshots of each step will be added with the first GUI release.
