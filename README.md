# Liberty_MeshMess
A PCB to make any LoRa module useful.

PCB Design © 2024 by NomDeTom is licensed under CC BY-NC-ND 4.0

## Use Case
Maybe you bought some radio modules on a whim? Maybe you clicked the wrong thing on Aliexpress. Maybe you couldn't make up your mind whether you wanted 22db or 30db, and bought both. Maybe you just want to try *all the things*.

Most PCB makers will only sell you boards in multiples of 5. OSHPark will only sell in multiples of 3. Either way, if you only have one module, you've got some spares.

This board will allow you to try lots of different things.

It accepts a Pro-micro, or can be used as a Pi-hat. If you use the one with Ellis Pi-land attached, you can also use a Pi-Pico.

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

The battery ADC 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcxMTQwNDI3NV19
-->