# Liberty_MeshMess
A PCB to make any LoRa module useful.

PCB Design © 2024 by NomDeTom is licensed under CC BY-NC-ND 4.0

If this is interesting, check out my other stuff:

[Femtofox](https://github.com/Nestpebble/Femtofox_Community_Hardware)

[NiceRa Pro Micro Nodes](https://github.com/Nestpebble/NiceRa)

![Liberty MeshMess](https://raw.githubusercontent.com/Nestpebble/Liberty_MeshMess/refs/heads/main/assets/meshmess_front.webp)
![Liberty MeshMess](https://raw.githubusercontent.com/Nestpebble/Liberty_MeshMess/refs/heads/main/assets/meshmess_back.webp)


## Use Case
Maybe you bought some radio modules on a whim. Maybe you clicked the wrong thing on Aliexpress. Maybe you couldn't make up your mind whether you wanted 22db or 30db, and bought both. Maybe you just want to try *all the things*.

Most PCB makers will only sell you boards in multiples of 5. If you only have one module, you've got some spares. This board will allow you to try lots of different things, all on the same board.

It accepts an NRF52840 Pro-micro, or can be used as a Pi-hat. If you use the one with Ellis Pi-land attached, you can also use a Pi-Pico.

Why is it called Liberty? Because it accepts all your modules, almost regardless of type.

Why is it called MeshMess? Have you looked at it‽‽‽

## BOM
Modules supported:
#### CDEbyte
- E22-900M30S *
- E22-900M22S *
- E22-900MM22S *
- E80-900M2213S
#### AI-Thinker
- RA-01SH
#### Heltec
- HT-RA62
#### Seeeed
- WIO SX1262
#### NiceRF 
- Lora1262

### Parts needed
If you are using an ebyte E22 module (one marked with a * above), you will need 2x 100kΩ resistors, 1x N-channel mosfet, and 1x P-channel mosfet. This runs the automatic RF switching.

If you are using any of the other modules, those parts are unnecessary.

If you're using a WIO SX1262, you will need to adjust the PiPico variant firmware to accept RXEN on GPIO18.

The battery ADC for the Pro-Micro requires 1x 220kΩ and 1x 330kΩ resistor.

The battery ADC for the PiPico requires 2x 500kΩ resistors or similar.

The Ebyte E22-900M30S requires 5V to operate, which has to be supplied using the JST connector if you're using a Pro-Micro. I've protected the battery pin on the Pro-Micro with a diode. Forward voltage drop on the diode should ideally be 0.8-1.5V. A shawty diode can be used, but you might want to use a couple in series to get the drop needed.

### Variations on parts
You can use 1206, 0805 or 0603 size resistors, or you can use through-hole. Only use one size at a time!

You can use SOT23 mosfets, or through-hole ones. SOT23 are pretty fixed footprints, but pay attention to the pins on TO92 type ones - they can be tricksy. Again, only use one type per position!

### Future expansion
You'll notice the schematic has a couple of crossed-out boards. Yeah, I couldn't be bothered to add them all. Maybe later?
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzMDkzNTgwNSwtMTU5NzE2NDMxMSwxMz
MwOTAxOTM5LC0xMTgxNjEwMjIxXX0=
-->