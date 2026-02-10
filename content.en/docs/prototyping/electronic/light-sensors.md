---
weight: 3
title: Light Sensors
---
# Light Sensors

>[!SUCCESS]
> **Goal.** Build a simple light-sensitive circuit where the LED turns on when it gets dark—like a tiny automatic night light.

## Instructions for TinkerCAD

<iframe width="100%" height="600px" frameborder="0" allowfullscreen="" src="https://dubble.so/guides/light-sensors-wbjg27cs33opxipfolqi?embed=1"></iframe>

## Components

- Breadboard
- 1x LED
- 1x resistor (220Ω for the LED)
- 1x LDR (light-dependent resistor)
- 1x resistor (10kΩ) – for the voltage divider
- 1x NPN transistor (e.g. BC547 or 2N2222)
- 1x battery pack (e.g. 2xAA or 9V)
- Jumper wires
## Key concepts

- **LDRs** change resistance based on light:
	- **Bright light = low resistance**
	- **Dark = high resistance**
- A **voltage divider** turns this resistance change into a voltage signal.
- A **transistor** acts like an electronic switch to turn the LED on or off depending on that signal.
## Step-by-Step Instructions

{{% steps %}}
1. ### Set Up the Voltage Divider
   This is how we “read” the LDR’s signal.
   - Place the **LDR** across two rows of the breadboard.
   - Connect one end of the **10kΩ resistor** to the **same row as one side of the LDR**.
   - Connect the **other end of the resistor** to **ground (–)**.
   - Connect a **jumper wire** from the **middle point** (where the LDR and 10k resistor meet) to the **base** of the **NPN transistor**. This “middle point” gives a voltage that changes with light.

2. ### Connect Power to the LDR
   Connect the **other end of the LDR** (not shared with the resistor) to **+ (positive)** on the battery.
3. ### Set Up the LED and Transistor
	- Place the **LED** on the breadboard (long leg to one row, short leg to another).
	- Connect the **short leg (–)** of the LED to the **collector** of the transistor.
	- Connect the **emitter** of the transistor to **ground (–)**.
	- Place a **220Ω resistor** between the **long leg (+)** of the LED and **+ power** from the battery.

4. ### Power It On and Test
	- Insert batteries or connect the battery clip.
	- **Cover the LDR** with your hand.
	- The LED should **turn on in the dark** and **turn off in bright light**.
{{% /steps %}}

## What you’ve learned

- LDRs let your circuit **react to the environment**.
- A **transistor** acts as a bridge between a weak signal and a stronger action (like lighting an LED).
- You’ve now used a **sensor to control a circuit**—no programming needed!

## Try this

- Reverse the logic: can you make it turn **off in the dark** and **on in the light**?