# slabV Build Guide

Once you have all the parts, construction is pretty simple.  Please
take a look at the parts list to get oriented:
[Parts list (BOM)](../docs/bom.md)

Some of the construction descriptions make this whole thing sound
more complex than it really is.  Take a look at the 
[images](../images)
 and it hopefully all make sense.  Email with any questions!

## Flash

Start by flashing the firmware to the MCU just to make sure it's 
working properly.  This will also allow you to test the footprints
when you are done soldering the diodes and MCU.  

The slabV uses the same pinout and matrix as the chocV.  You can use
any of the precompiled .hex files in the 
[chocV repo](https://github.com/brickbots/chocV/firmware) or build
from source using the chocV files in the main QMK repo.

## PCB 

Start by soldering the surface mount diodes on the bottom 
side of the PCB.  The bottom plates have cut-outs for these
diodes and legs of the top-side through hole components.  There
should be enough room to accomidate some misplacmenet or big solder 
joints, but take care and be tidy.  Polarity of the diodes is marked
on the pcb with line which should be on the same side as the line 
on the diodes. 

Once you have the diodes soldered on, I suggest doing a quick
test fit of the bottom acrylic piece to make sure all the cut-outs
line up nicely.  If any of the diodes are askew or rub on the 
edge of the cut-outs, now's the time to fix them up.  

Then move on to the microcontroller on the top side.  Feel free to 
socket or solder it directly... but make sure to mind the pinout!
The MCU is mounted 'upside down' with the components facing the PCB.

Because of the construction here, I very much recommend using sockets
for the switches. The PCB will fit millmax or similar sockets and the 
ability to remove the switches when layering up the case can be handy.
It can definitely be done soldered, but take care to layer up the 
pieces correctly and make sure the standoffs are installed and 
screwed in prio to soldering in the switches.  The stand-offs are 
captive between the PCB and the top layer of acrylic, so once you
solder in switches you can't insert them.  If I were to make one 
revision, it would be to increase the diameter of the PCB holes to 
allow the stand-offs to pass through.

Once the diodes and MCU are in place it's a good a good time to 
test all the switch footprints to make sure everything is looking
good.  Because the acrylic of the case is sandwiched between between
the PCB and the switch housings it gets increasingly difficult to 
fix problems if you have not opted for hot-swap sockets.  

## Switches / Mid & Top layers


### A note on the 3mm M2 female/female standoffs
There is about 3mm of space between the PCB and the top acrylic 
layer (2 x 0.5 silicone layers and one 2mm acrylic piece) if 
all the layers are exactly at spec. Ideally, you'll want your 
stand-offs to be a bit shorter than the distance between the PCB
and the bottom of the top acrylic piece so that as you tighten 
the screws it's compressing the silicone rather than tightening
against the actual stand-offs.

Your acrylic pieces and stand-offs will probably have some 
variance,  so you may have to adjust/experiment here.  My 3mm M2 
stand-offs were actually a bit longer than 3mm and didn't allow the 
silicon to compress properly. 

I ended up using some 3mm M2 brass threaded hot-set inserts which were 
just a bit shorter than 3mm.  These are often used to coupling metal 
fasteners to 3d printed parts.  They are pretty much stand-offs with a 
knurled outside surface.  So be creative here with the hardware choices.

If you have not opted for hot-swap sockets, you'll need to make sure
the four middle layers are placed between the PCB and the switch tops 
before soldering in the switches. I recommend building the layers 
'upside down' and making sure the stand-offs are properly placed.

Start with the TOP layer with the smaller screw holes and insert
the male ends of the 4 M2 3mm male/female standoffs through the 
screw positions around the central cutout for the MCU.  These will 
suppor the MCU cover later.  Secure these on the other side with 4 
of the 3mm female/femal stand-offs.

Next, use 8 of the M2 3mm screws to secure the remaining 3mm 
female/female stand-offs to the top acrylic piece.

Startng with one of the mid-layer silicon gaskets, fit it over the 
stand-offs sticking out the bottom of the top acrylic layer, then a 
place a mid-layer acrylic piece, then one more mid-layer gasket. 

You can now temporarily secure the PCB to the top stack using some 
shorter m2 screws.  You don't need them all, just enough to hold 
the stack and PCB together so you can insert and solder the switches.


## Bottom Layers 

Once you have switches soldered, or have inserted sockets, you can
remove the temporary screws and place the bottom silicon gasket and
acrylic piece under the PCB.  The cutouts are not symmetrical so you
may need to flip the pieces to get them to line up properly with the 
PCB.  Use the longer 6mm M2 screws from the bottom to secure the 
whole thing together.  

Put on some feet and the top MCU cover and you should be good to go! 
If the board does not site flat on a tabletop, loosen a few of the 
screws and you should be able to gently bend/twist the whole assmebly 
until it's flat.  This depends a lot on your acrylic layers, PCB, etc, 
but you should be able to get it all sorted and then tighten down the
screws again to secure it.

Feel free to contact me with any questions on building, 
flashing or aquiring parts.  If you do build on of these
I'd love to see it.
