# Klicky-FBG6
Klicky endstop for **Flying Bear Ghost 6**

Based on the [Condor Head for FBG6](https://github.com/Chiffa-C3/FBG6-Condor-C3) by [Chiffa](https://github.com/Chiffa-C3) which is based on the well-knopwn [Klicky-Probe by Jlas1](https://github.com/jlas1/Klicky-Probe). It gives Flying Bear Ghost 6 standard (stock) printer head klicky-probe support.

I took the back plate from the excellent job from [Ryoko](https://www.thingiverse.com/thing:5744744) (originally for 3d-touch) and modified it deeply to achieve the results needed.

<img src="/pics/FinalResult.jpg" height="400">

This design includes four parts:
- **Klicky-Probe** (which jumps from the printer head to the dock and viceversa)
- **Klicky-Dock** (the part where the probe usually remains. The Dock is attached to the dock-support)
- **Dock-Support** (attached to the chamber fan)
- A new **Back-Side** of the printer head box to replace the stock one, and where Probe is attached when needed.

You could download STL or STEP files from their respective folders. And with STEP files, if you know how, you could make modifications to my design if you wish.

## Printing settings

<img src="/pics/PrintBed.png" width="600">

I used ABS (Sunlu Gold) for printing, 0.4mmm nozzle.
- Layer Height 0.12mm (probably 0.20mm will work right too)
- Supports are needed just for Dock-Support and Back-Side
- 25% infill sparse density (I prefer Gyroid type)
- Brim just if you need it

## Material needed
**Back-Side**
- 2 x M3 Brass Insert Nuts Length 5-6mm Outer Diameter 4-4.5mm
- 3 x round magnet 5x5mm
- 2 x thin wire (less than 0.5mm) of around 1-1.5 meters
- 1 x XH2.54 3 pin connector to connection to the motherboard with 2 female pins or reuse an older sensor cable, or put 2 female dupont connectors to the motherboard side)

**Dock-Support**
- 2 x M3 Brass Insert Nuts Length 4-5mm Outer Diameter 4-4.5mm
- 1 x round magnet 5x5mm
- 4 x M3 hex head bolts 14-16mm length to replace the fan bolts

**Klicky-Dock**
- 2 x M3x20mm screws (hex or round head)

**Klicky-Probe**
- 2 x M2 hex self-tapping bolts length 6-8mm
- 4 x round magnet 5x5mm
- 1 x microswitch (D2F) recommended or a [cheap](https://www.aliexpress.com/item/4001033375208.html?spm=a2g0o.order_list.order_list_main.17.319318023T0rvD) alternative

### Tools needed
- Hex head screwdriver set
- Cyanoacrylate glue (Loctite, SuperGlue...)
- Crimper (if you will make your motherboard connectors)
- Iron Solder (to install the insert nuts and solder the wires if you reuse an old connector to the motherboard)

## Assembly

### Install the insert nuts

Use an iron solder for this job, with heated head, push lightly the inserts into the corresponding holes. When a little less than 1mm is missing, push the inserts with a flat piece of metal to give a perfect finish. You'll need to do this job just 4 times (in Back-Side and Dock-Support), so keep calm and do it right.

### Install the Dock-Support and Dock
<img src="/pics/DockSupport.png" height="200">

Unscrew the 4 bolts of the rear fan, and install the Dock-Support over it with the connection to the dock down.

Insert one magnet in the rear of the Klicky-Dock (here you won't need to glue it) and connect it with 2 M3x20mm to the Dock-Support.

This is the piece finished:
![Dock-Spics/photo_2024-01-12_18-46-01.jpg

### Install the Back-Side
First unscrew the stock backside (2 M3 bolts that you could reuse for installing the new one later).

<img src="/pics/Klicky-Holder-Poles.png" width="200">

To start, you must take note that there are 3 magnets on the downside of the piece, two of them (A and B) will have a wire connection and the third (C) helps the klicky so it doesn't spin or been loosed. The two wired magnets (A and B)) should have the same pole (North or South, but both the same), pointing to the exterior and the third magnet (C) must have the pole interchanged with them (so if the wired magnets are pointing North, this must be pointing South).
You could discover the pole of every magnet with some mobile applications but you don't really need them if you use a bit of common sense so:

- if you install magnet A, you could link another magnet to it and **without rolling/spinning** it, you could transfer directly to the hold B and insert it, both will expose the same pole.

In the same way, you could link a third magnet to any of A or B, rotate it and insert on C hole, so it will expose the opposite pole than A and B.

Pass the wires through the center holes up-down direction, strip ~10mm on each wire and (IMPORTANT!!! not spin/rotate the wires, you need them plain to let the magnets been introduced in their holes), and gently push them to the magnet holes so when you put the magnets inside, the wires been pressed by them. Before installing the magnets, put a drop of glue in the holes so they wont been loosed. REMEMBER! These 2 magnets (A and B) should expose the same pole and the third the opposite pole.

<img src="/pics/photo_2024-01-12_18-46-01.jpg" width="400">

Then, you could install it in the printer head passing the wires through the hole (like the [picture](/pics/photo_2024-01-12_18-45-59.jpg)), take them up to the motherboard and connect it to the Z-MAX connector (PC4).

### Mount the Klicky-Probe
<img src="/pics/photo_2024-01-12_18-46-14B.jpg" width="300">

First, you should install the microswitch in its place and fix it with the screws. Then you should put three magnets which will go upside, an easy way is to attach three magnets to the magnets installed yet on the Back-Side and push the Klicky-Probe over them, this will ensure they are right oriented. First, to secure them, it should be better to put a drop of glue on the holes.

It's required that the outer legs of the microswitch have good contact with the magnets.

<img src="[/pics/photo_2024-01-12_18-46-14B.jpg](https://github.com/Chiffa-C3/FBG6-Condor/blob/main/Assembly/PIC/pic10.png)" width="300">

In this way, the swich system should work, and you could test it: with a multitester with continuity measurement, you could check there is continuity between A and B magnets, but if you push the switch, continuity is loosed.

You now could put another drop of glue in the back side hole and put the fouth magnet (as it should be related to the one on the Dock, you could link a magnet in the Dock and push the Probe over it to install the magnet).

### End of Assembly part

Now, you just need to put the Probe on its dock, give a few clockwise turns to the old Z endstop screw to download it and prevent it to touch the old switch, and start with the software configuration.

## Software Configuration

This manual is intended to work just with **Klipper** so, if somebody wants to write a Marlin manual, it'll be welcome and I could publish here.

###Klipper files

We use original klipper macros from jlas1 that you could find [here](https://github.com/jlas1/Klicky-Probe/tree/main/Klipper_macros), or downlad directly all of them together through [his zip file ](https://github.com/jlas1/Klicky-Probe/tree/main/Klipper_macros/Klipper_macros.zip).

An easy way to install them is connecting through ssh, change directory to the config folder from our printer and:

```ShellSession
mkdir klicky
cd klicky
wget https://raw.githubusercontent.com/jlas1/Klicky-Probe/main/Klipper_macros/Klipper_macros.zip
unzip Klipper_macros.zip
```
In this way, we have all the klicky related files together in a folder, making a cleaner installation.

There are a few files there, but the more important is **klicky-probe.cfg** from which we will indicate Klipper which of them will load. For my configuration, I uncommented variables, macros, bed-mesh-calibrate and screws-tilt-calculate:

```python
#Simple way to include all the various klicky macros and configurations
# the current home for this configuration is https://github.com/jlas1/Klicky-Probe, please check it

#[include ./klicky-specific.cfg]                #place to put other configurations specific to your printer
[include ./klicky-variables.cfg]                #Required
[include ./klicky-macros.cfg]                   #Required
[include ./klicky-bed-mesh-calibrate.cfg]      #bed mesh, requires klipper configuration
[include ./klicky-screws-tilt-calculate.cfg]   #help adjust bed screws automatically
#[include ./klicky-quad-gantry-level.cfg]       #level 4 Z motors
#[include ./klicky-z-tilt-adjust.cfg]           #level 2 or 3 Z motors
```
Or you could just replace the original file [with mine](/cfg/klicky-probe.cfg).


Now, we will edit the file **klicky-variables.cfg** and change these variables to adapt it to our printer:

```python
variable_max_bed_y:            200
variable_max_bed_x:            250
variable_z_endstop_x:         0
variable_z_endstop_y:         0
variable_docklocation_x:      168
variable_docklocation_y:      215
variable_docklocation_z:      -128
Variable_dockmove_x:            30
Variable_attachmove_x:           0
Variable_attachmove_y:          17
variable_park_toolhead:       True
variable_parkposition_x:         1
variable_parkposition_y:         1
variable_parkposition_z:        10
variable_home_backoff_x:     125.5
variable_home_backoff_y:      70.5
```
Or you could just replace the original file [with mine](/cfg/klicky-variables.cfg).

Now, you could upload my [klicky.cfg](/cfg/klicky.cfg) file to the same klicky folder. It contains the configuration for out klicky probe:
```python
[probe]
pin: ^PC4
x_offset: 2.5
y_offset: 35.5
speed: 5.0
lift_speed: 15.0
samples: 3
sample_retract_dist: 1.0
samples_result: average
samples_tolerance: 0.1
samples_tolerance_retries: 6

[bed_mesh]
speed: 100
horizontal_move_z: 5
#mesh_min: 7.5, 35
mesh_min: 12.5,45.5
#mesh_max: 240, 200
mesh_max: 246.0,205.0
probe_count: 6,5
mesh_pps: 2, 2
algorithm: bicubic
fade_start: 1
fade_end: 10

[screws_tilt_adjust]                     
screw4: 25, 1
screw4_name: Left-Front
screw3: 225, 1
screw3_name: Right-Front
screw2: 225, 145
screw2_name: Right-Back
screw1: 25, 145
screw1_name: Left-Back
speed: 200
screw_thread: CW-M4
horizontal_move_z: 5
```
As you could see, I defined a **bed_mesh** section to could calibrate the printer hotbed, and a **screw_tilt_adjust** for helping us to adjust the bed screws. It's configured using the max distance I could achieve with the nozzle in my printer (it shouldn't change in others FBG6 printers). To achieve all those points, you should change our **printer.cfg ** with the data in their respective sections:
```python
[stepper_x]
...
position_max: 256

[stepper_y]
...
position_max: 215

[stepper_z]
...
endstop_pin: probe:z_virtual_endstop
```
See the last change is to let our new klicky probe take control of the limit in Z height,

Finally, we should edit our **printer.cfg** file again and activate our files for the changes to take effect. Better after every other **include** in the file:
```python
[include klicky/klicky.cfg]
[include klicky/klicky-probe.cfg]
```
Note that the last include will make everyother needed files (macros, bed-mesh-calibrate and screws-tilt-adjust) been imported too.

We should add one line for the probe to let it change later at calibration:

```python
[probe]
z_offset = 2.380
```

After restarting Klipper, we should start doing some tests from the klicky macros in the klipper console with these simply commands:
- **ATTACH_PROBE**
- **DOCK_PROBE**

If both commands worked right, we could **home** our head wishing everything will be all right.

After that, there are a few useful commands:
- **PROBE_ACCURACY**     ===> to test the accuracy of our probe, look at the **range** exit. For our machines, a range of 0.0025 is acceptable.
- **PROBE_CALIBRATE**    ===> to calibrate the distance between nozzle and klicky probe, just usual
- **BED_MESH_CALIBRATE** ===> to probe the bed with the points defined and make a mesh to print better.

See the klicky in action with the Flying Bear Ghost 6:


https://github.com/ColdBeer72/Klicky-FBG6/assets/78320296/a434295b-317d-4c4f-b1c3-35d6b134ba49

