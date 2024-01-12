# Klicky-FBG6
Klicky endstop for Flying Bear Ghost 6

Based on the [Condor Head for FBG6](https://github.com/Chiffa-C3/FBG6-Condor-C3) by [Chiffa](https://github.com/Chiffa-C3) which is based on the well-knopwn [Klicky-Probe by Jlas1](https://github.com/jlas1/Klicky-Probe). It gives Flying Bear Ghost 6 standard (stock) printer head klicky-probe support.

This design includes four parts:
- **Klicky-Probe** (which jumps from the printer head to the dock and viceversa)
- **Klicky-Dock** (the part where the probe usually remains. The Dock is attached to the dock-support)
- **Dock-Support** (attached to the chamber fan)
- A new **Back-Side** of the printer head box to replace the stock one, and where Probe is attached when needed.

## Printing settings

I used ABS (Sunlu Gold) for printing, 0.4mmm nozzle.
- Layer Height 0.12mm (probably 0.20mm will work right too)
- Supports are needed just for Dock-Support and Back-Side
- 25% infill sparse density (I prefer Gyroid type)
- Brim just if you need it

## Preparation

### Material needed
**Back-Side**
2 x M3 Brass Insert Nuts Length 5-6mm Outer Diameter 4-4.5mm
3 x round magnet 5x5mm
2 x thin wire (less than 0.5mm) of around 1-1.5 meters
1 x XH2.54 3 pin connector to connection to the motherboard with 2 female pins or reuse an older sensor cable, or put 2 female dupont connectors to the motherboard side)

**Dock-Support**
2 x M3 Brass Insert Nuts Length 4-5mm Outer Diameter 4-4.5mm
1 x round magnet 5x5mm
4 x M3 hex head bolts 14-16mm length to replace the fan bolts

**Klicky-Dock**
2 x M3x20mm screws (hex or round head)

**Klicky-Probe**
2 x M2 hex self-tapping bolts length 6-8mm
4 x round magnet 5x5mm

### Tools needed
- Hex head screwdriver set
- Cyanoacrylate glue (Loctite, SuperGlue...)
- Crimper (if you will make your motherboard connectors)
- Iron Solder (to install the insert nuts and solder the wires if you reuse an old connector to the motherboard)

## Assembly



### Preparation

### Install the insert nuts

Use an iron solder for this job, with heated head, push lightly the inserts into the corresponding holes. When a little less than 1mm is missing, push the inserts with a flat piece of metal to give a perfect finish. You'll need to do this job just 4 times (in Back-Side and Dock-Support), so keep calm and do it right.

### Install the Dock-Support and Dock
![Image of Dock-Support](/pics/DockSupport.png)

Unscrew the 4 bolts of the rear fan, and install the Dock-Support over it with the connection to the dock down.

Insert one magnet in the rear of the Klicky-Dock (here you won't need to glue it) and connect it with 2 M3x20mm to the Dock-Support.

### Back-Side
First unscrew the stock backside (2 M3 bolts that you could reuse for installing the new one later).

![Image of the Klicky Holder](/pics/Klicky-Holder-Poles.png)
To start, you must take note that there are 3 magnets on the downside of the piece, two of them (A and B) will have a wire connection and the third (C) helps the klicky so it doesn't spin or been loosed. The two wired magnets (A and B)) should have the same pole (North or South, but both the same), pointing to the exterior and the third magnet (C) must have the pole interchanged with them (so if the wired magnets are pointing North, this must be pointing South).
You could discover the pole of every magnet with some mobile applications but you don't really need them if you use a bit of common sense so:

- if you install magnet A, you could link another magnet to it and **without rolling/spinning** it, you could transfer directly to the hold B and insert it, both will expose the same pole.

In the same way, you could link a third magnet to any of A or B, rotate it and insert on C hole, so it will expose the opposite pole than A and B.

Pass the wires through the center holes up-down direction, strip ~10mm on each wire and (IMPORTANT!!! not spin/rotate the wires, you need them plain to let the magnets been introduced in their holes), and gently push them to the magnet holes so when you put the magnets inside, the wires been pressed by them. Before installing the magnets, put a drop of glue in the holes so they wont been loosed. REMEMBER! These 2 magnets (A and B) should expose the same pole and the third the opposite pole.

### Klicky-Probe
