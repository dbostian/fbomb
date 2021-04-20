# F Bomb
## A 3d Printed Macropad

![example](https://i.imgur.com/6fZqQ7q.jpg)

![example](https://i.imgur.com/M7bTRSy.jpg)

**Designer's Note:** This project is an exploration of the theme *Information as a Weapon*. 

## Intro
A 3d-printable macropad for your Fn enjoyment. It contains 12 Fn keys for your favorite Fn macros.

Why did I design this? I've been building a few 40% and 60% keyboards lately, and I've discovered I have a growing collection of Fn row keycaps with no Fn use. What should I do with all these Fn keys? A Fn macropad, of course! But why settle for a rectangular Fn keypad?


## Project Structure
**/stls** - STL files for 3d Printing

## Construction

### Printed Parts
- [ ] 1x Shell
- [ ] 1x Base
- [ ] 1x Fuse

### Hardware
- [ ] 12x Keycaps. Whatever Fn caps you have lying around.
- [ ] 12x Switches, presuming they fit in a 14mm square square hole. Cherry MX or compatible.
- [ ] 12x 1N4148 Diodes
- [ ] 1x Pro Micro
- [ ] Crimp terminals, housings (3 pin, 4 pin)
- [ ] 4x M3 x 8mm Countersunk Machine Screw
- [ ] 1x M3 x 12mm Socket Cap Machine Screw
- [ ] VHB or other double-stick tape (optional)
- [ ] Wire
- [ ] Heat Shrink Tubing

### Tools / Misc
- [ ] 3d Printer + Filament
- [ ] Soldering Iron + Solder
- [ ] Multimeter
- [ ] Wire Cutters / Strippers / Flush Cutters
- [ ] Crimping Pliers
- [ ] Hex Drivers

### Printing Notes
I printed mine at 0.2mm. The shell needs support - a lot of Fn support - but the base and fuse do not.

### Assembly
Install heatset inserts into the fuse and shell. Attach the fuse to the shell with an M3 x 12mm screw from the inside. It's best to do this before you Fn wire it.

![example](https://i.imgur.com/VzRUuUW.jpg)


### Wiring
I wired my macropad into a 4x3 matrix. Each switch gets a diode and ~100mm of wire. I did not want to reach a soldering iron inside the Fn shell.

I used Red for Rows, and blaCk for Columns. Each column wire gets a flag with a number, 1-4. I inserted the first row of four switches, and spliced the row wires together. This then went into a crimped conenctor. I repeated this for the remaining two rows, and then all of the matching columns. You do not want two switches with the same row + column.


![example](https://i.imgur.com/LSr06mr.jpg)

![example](https://i.imgur.com/hxK1lkm.jpg)

![example](https://i.imgur.com/Uq13ZOQ.jpg)

![example](https://i.imgur.com/TrE1leO.jpg)

![example](https://i.imgur.com/48OkCIF.jpg)


### Microcontroller + Firmware
Solder headers onto a Pro Micro and snap it into the Fn base as shown. I like to use a strip of VHB double stick tape to keep it from rattling loose.
![example](https://i.imgur.com/zVHjH0B.jpg)

Attach the matrix, figure out what pins you've picked, and flash that Fn thing. I use [QMK firmware](https://qmk.fm/)

If all the Fn keys work, shove the wires into the shell as best you can, and screw on the base. Give yourself a Fn high five.
