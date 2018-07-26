https://imgur.com/a/bGH9G0s

# Quefrency Build Guide

## Parts List

Here's a list of parts needed for the build:

* 1 [Quefrency PCB Kit](https://keeb.io/collections/split-keyboard-parts/products/quefrency-60-split-staggered-keyboard)
  * 2 Reset Switches \(included in kit\)
  * 2 4.7kΩ resistors \(included in kit\)
  * 2 TRRS Jacks \(included in kit\)
  * 47 1N4148 diodes - through hole \(included in kit\) and [SMD diodes]((https://keeb.io/products/1n4148-diodes) supported

* 1 [Quefrency Case Plates](https://keeb.io/collections/split-keyboard-parts/products/quefrency-60-split-staggered-keyboard)
  * 29 M2 6mm screws \(included with plates\)
  * 14 M2 10mm standoffs \(included with plates\)
  
* 2 [Arduino Pro Micros](https://keeb.io/products/pro-micro-5v-16mhz-arduino-compatible-atmega32u4)
* 1 TRRS Cable()
* 1 Micro USB Cable()
* PCB-mount MX stabilizers()
* MX or Alps compatible keyswitches
* WS2812B Compatible RGB LED strip](https://keeb.io/collections/frontpage/products/rgb-led-strips-sk6812-ws2812b-compatible) \(optional, for underglow\)

## Build Steps

1. Prepare components
2. Solder components
    * Solder diodes
    * Solder push button
    * Solder 4.7kΩ resistors \(optional\)
    * Solder Pro Micro header pins
3. Solder switches
4. Flash Pro Micro
5. Solder Pro Micro
6. Solder RGB strip \(optional\)

## Prepare Components

![](https://i.imgur.com/x96LIyE.jpg)

Get your parts all set and make sure you have all the components.

![](https://i.imgur.com/h7aNdeq.jpg)

Make sure to let kitty know it's build time, if you don't she'll forget to disrupt you every step of the way.

[]!(https://i.imgur.com/NXZVbjx.jpg)

If you're using through hole diodes, bend 'em up. Here, I'm just bending it around my finger. Then tear the paper off carefully as not to bend them.

![](https://i.imgur.com/E6WgUsd.jpg)

Insert the diodes. The orientation of all the diodes are the same, they are vertically oriented, with the band on the diodes facing towards the bottom, square pad.

Through-hole diodes will have a black band, SMD diodes have a white band.

**Note**bakingpy suggests always installing the diodes on the bottom of the PCB. This way, if a diode goes bad, it's very simple to replace. If you choose to install them on the top, should any go bad, you will regret this. I've done it before, I hope never to do it again, yet I put them topside for some reason. Don't be me, listen to bakingpy's advice!

![](https://i.imgur.com/XNP7s38.jpg)

All the diodes installed on the left PCB.

![](https://i.imgur.com/Ed8bK7H.jpg)

After installing the diodes, add your TRRS jacks and reset buttons.

![]https://i.imgur.com/Ed8bK7H.jpg)

Add your 4.7k ohm resistors for i2c on the left half(optional). There are no resistors for the right half. Resistors also do not have a polarity, so the orientation doesn't matter when placing them.

![](https://i.imgur.com/1s2MgQZ.jpg)

Repeat the same process with the diodes, TRRS jack, and reset switch with the right half. Remember no I2C resistor slots on this side, as they're only needed on one half. Then, take a moment to pet kitty before she hates you for ignoring her.

## Solder Components

![](https://i.imgur.com/AiDoJdn.jpg)

Solder on the header pins for the Pro Micro.

First technique: Put on first row of header pins and solder one pin. Then check to see if it's aligned properly before soldering the rest of the row.

![](https://i.imgur.com/LKaHUuV.jpg)

Alignment after first row is good, solder the rest of the pins.

![](https://i.imgur.com/NvHFYqh.jpg)
1

Same thing with the other row of header pins, solder one pin first, check alignment, then solder the rest.

![](https://i.imgur.com/62jgd90.jpg)

Second technique for soldering header pins on: Tape row of pins so they stay in place while you solder them in.

![](https://i.imgur.com/tRwjwFZ.jpg)

Repeat for the other row of pins.

![](https://i.imgur.com/nU47rLi.jpg)

![](https://i.imgur.com/FMhd0WO.jpg)

Due to the location of the stabilizers on the right half, the Pro Micro header pins needed to be situated a bit lower than usual. This interferes a bit with one of the switches, so the pins need to be trimmed down a bit on that side.

![](https://i.imgur.com/JrxztrO.jpg)

Another view which shows the pins that will need to be trimmed down.

![](https://i.imgur.com/JUJuRle.jpg)

Take a flush cutter to trim the pins down.

![](https://i.imgur.com/IQnHd0Y.jpg)

All good now, the switch sits flat on the PCB.

![](https://i.imgur.com/ORDwvw1.jpg)

Add stabilizers to the keys you want to stabilize.

![](https://i.imgur.com/ysM9w7t.jpg)

Time to add the switches. Put a few switches into the corners of the switch plate and then attach the switches to the PCB. Make sure the switches are pushed all the way down onto the PCB.

Due to the multiple layout options, it may be helpful to put keycaps on the switches to make sure everything is in the correct slots.

![](https://i.imgur.com/ZcmuoHR.jpg)

If you paid attention closely to the previous picture, the lower left switch was too close to the one to the right of it to properly do a 4x1u configuration on the bottom row. Turns out I forgot to expand the cutout width when I added support for that configuration. This has already been fixed in the next version of the plates.

![](https://i.imgur.com/nOM9XWl.jpg)

All the switches installed and soldered in.

![](https://i.imgur.com/kaxSMbD.jpg)

Time to install the Pro Micro now that the switches have been soldered in.

![](https://i.imgur.com/Y8LYgMx.jpg)

To make sure that the switch pins don't touch the Pro Micro, clip them flush with the PCB.

![](https://i.imgur.com/wD2B0Te.jpg)

Afterwards, add Kapton or electrical tape on top of it.

Now go flash your Pro Micro before installing it on the board. Better to find out if it's defective or not before it's soldered on.

![](https://i.imgur.com/Zjbn2GT.jpg)

Place the Pro Micro on the header pins. On both PCBs, the component side of the Pro Micro will be hidden from you.

Don't install it backwards, it doesn't flip the layout or anything like that, it doesn't work in that way.

![](https://i.imgur.com/g5XCCqr.jpg)

Repeat the process of stabilizer, switch, and Pro Micro installation on the right PCB.

![](https://i.imgur.com/Qtoo3b9.jpg)

Once again, the component side of the Pro Micro will be hidden from you.

![](https://i.imgur.com/DuXct1J.jpg)

Optional, add RGB strip. For the left half here's what to connect:
- RGB breakout goes to Din on strip
- VCC breakout goes to +5V on strip
- GND breakout goes to GND on strip
- Extra Data goes to Do/Dout on strip

![](https://i.imgur.com/cJ1Czig.jpg)

Pro Micro added to the right PCB. Here's what to connect for the right half:
- VCC breakout goes to +5V on strip
- GND breakout goes to GND on strip
- Extra Data goes to Din on strip
- RGB breakout remains empty for now

![](https://i.imgur.com/DIqF3bf.jpg)

Assemble the case by adding screws, standoffs, and bottom plates.
