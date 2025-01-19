Attention, the project is under development, so it is subject to change.

# LumiTimeV2

LumiTimeV2 - this is the "Perpetual" Wristwatch(project code name "LumiTimeV2") with 12 red LEDs, it have LIR3032 Li-Ion battery and 12 solar cells, based on a Microchip microcontroller ATmega328P. It's full open source(firmware and hardware).

Next generation wristwatch after [12 LED ATtiny "Perpetual" Wristwatch](https://github.com/techn0man1ac/PerpetualLEDWristwatch). 

# Video demonstration:

/* Link may be here */

# How it's work?

/* Description may be here */

# How to set the time?

/* Description may be here */

# 3D model PCB:

The board is two-layer, with components on both sides. 

## PCB front view

On the front side of the board there are 12 microsolar panels in a circle and 12 red LEDs that display the time and the RTC with its quartz resonator:

![LumiTimeV2 PCB board render](https://raw.githubusercontent.com/techn0man1ac/LumiTimeV2/refs/heads/main/LumiTimeV2/img/LumiTimeV2BoardRender.png)

## Back view

In the center of the board is the ATmega328 microcontroller(like Arduino Nano). Under LED III is a button used to display and set the time for the watch. All passive components of the circuit are of 0805 size, which allows them to be soldered without additional soldering equipment:

![LumiTimeV2 PCB board render back](https://raw.githubusercontent.com/techn0man1ac/LumiTimeV2/refs/heads/main/LumiTimeV2/img/LumiTimeV2BoardRenderBack.png)

PCB have 35 mm in the diameter:

![LumiTimeV2 PCB board size](https://raw.githubusercontent.com/techn0man1ac/LumiTimeV2/refs/heads/main/LumiTimeV2/img/LumiTimeV2PCBSizes.png)

The thickness of the board is recommended to take 0.8mm otherwise it may not fit into the case.

# PCB gerber files:

Files for fabrication:

https://github.com/techn0man1ac/LumiTimeV2/tree/main/LumiTimeV2/PCB/Gerbers

# 3D model of PCB 

3D model in STEP format:

https://github.com/techn0man1ac/LumiTimeV2/tree/main/LumiTimeV2/PCB/3dModel

# Schematic

The circuitry of the clock provides for a sufficient number of parts, due to which the board is required to have parts on both sides. Here is a detailed description of each block on the schematic.

![LumiTimeV2 Schematic](https://raw.githubusercontent.com/techn0man1ac/LumiTimeV2/refs/heads/main/LumiTimeV2/img/LumiTimeV2Schematic.png)

## Charging system

The project uses 12 photodiodes BPW34S(PV array) that work like miniature solar panels, whose function is to charge the battery from light. 
The charging circuit is very primitive, since each micro-solar panel generates ~0.5V, if they are all 12 connected in series, the total voltage will be around 6 V, protect to overcharge the battery,used ZD1 Zener diode(4.7V), and a diode D13 is also prevent to reverse current(current flow into the solar panels) and add drop voltage 0.6-0.7V, as a result, we have a battery charging system with voltage like 4.0..4.1V. Charging current on a sunny day is ~2 mA.

## Battery

/* Description may be here */

## LEDs matrix

/* Description may be here */

## RTC

/* Description may be here */

## Programming connector

/* Description may be here */

## Microcontroller

/* Description may be here */

# Our mission and vision

It has a mission and vision that it borrowed from the [previous version](https://github.com/techn0man1ac/PerpetualLEDWristwatch) and carries the same values, such as:

## Mission:

To develop a simply and eco-friendly watch that integrates innovative technologies with minimal components, ensuring energy efficiency is within reach for all.

## Vision:

We aim to achieve a world where energy-saving technology is accessible to everyone, where our watch serves as a symbol of environmental stewardship and innovative solutions in energy efficiency.
