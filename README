# Analog LED Synth (Arduino + MCP3008)

An interactive LED instrument controlled by analog inputs.

This project uses an **MCP3008 ADC** and **Arduino** to read 4 potentiometers and transform them into expressive LED animations on an 8x8 matrix.

Instead of simple brightness control, each knob changes a behavioral parameter of the visual system — making this feel more like a playable device than a basic electronics demo.

---

## ✨ Features

* 4 Analog Controls via MCP3008
* Smooth parameter-based LED animations
* Multiple visual engines
* Designed for future custom PCB
* Expandable architecture

---

## 🎛️ Controls

| Potentiometer | Function           |
| ------------- | ------------------ |
| P1            | Pattern Type       |
| P2            | Speed              |
| P3            | Density            |
| P4            | Chaos / Randomness |

These parameters dynamically shape the animation instead of switching static modes.

---

## 💡 Visual Engines

The system blends between multiple animation styles:

* Flow Field (liquid motion)
* Cellular Automata
* Pulse / Breathing Patterns
* Spark / Firefly Movement

---

## 🧠 System Architecture

### Inputs

4x Potentiometers → MCP3008 → Arduino via SPI

### Outputs

8x8 LED Matrix driven by MAX7219

---

## 🔌 Wiring

### MCP3008 → Arduino

| MCP3008 | Arduino |
| ------- | ------- |
| VDD     | 5V      |
| VREF    | 5V      |
| AGND    | GND     |
| DGND    | GND     |
| CLK     | D13     |
| DOUT    | D12     |
| DIN     | D11     |
| CS      | D10     |

Potentiometers connect to:

* CH0
* CH1
* CH2
* CH3

---

### MAX7219 → Arduino

| MAX7219 | Arduino |
| ------- | ------- |
| DIN     | D11     |
| CLK     | D13     |
| CS      | D9      |

SPI lines are shared with MCP3008.

---

## 🧮 Parameter Mapping

Each potentiometer is normalized:

```cpp
float speed   = pot1 / 1023.0;
float density = pot2 / 1023.0;
float chaos   = pot3 / 1023.0;
float mode    = pot4 / 1023.0;
```

These values drive animation engines rather than acting as direct outputs.

---

## 🛠️ Hardware Requirements

* Arduino Nano / Uno
* MCP3008 ADC
* 4x 10k Potentiometers
* MAX7219 8x8 LED Matrix
* Breadboard + jumpers

---

## 🚀 Future Plans

* Custom standalone PCB
* ATmega328P onboard
* USB-C power input
* Optional preset button
* EEPROM preset saving
* NeoPixel version

---

## 🧩 PCB Vision

Planned layout:

```
[ POT ][ POT ]
[ POT ][ POT ]

[ 8x8 LED ]
```

Compact, synth-style interactive device.

---

## 📦 Project Status

Prototype phase — breadboard implementation.

Next step: schematic → PCB design.

---

## 🧪 Goals

* Learn SPI ADC integration
* Build parameter-driven UI
* Prepare for custom hardware manufacturing

---

## 📜 License

MIT
