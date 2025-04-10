
# __Trinity-toolhead__



I took inspiration from Takeoff, Calamity, Tiger's toolhead and IROB, and came up with this: 
A small footprint single-piece high performance toolhead option.

![trinity toolhead](https://github.com/user-attachments/assets/41433778-24b4-4971-bae2-0df017a28b86)



## This is currently untested, I am still working on it. I would love your feedback!

Discord: gerbz_

* The body is a single print to maximize weight, strength and stiffness.
* The hotend is supported at the bottom of the heatsink to increase stiffness.
* Double 3628 fans deliver enough cooling even for hot chambers.
* Optimised for dual gantry printers, the Y footprint of the toolhead itself is smaller than the sherpa mini.
* Light weight, estimated ~365g.
* The COM is on point!
  
![image](https://github.com/user-attachments/assets/4b7fee9b-9277-448e-b6ef-d20bfc20db1b)

## Recommended parts:
* 1x Fystec sherpa mini v3
* ~~bad~~ dragon ace volcano
* 2x Delta 3628
* 1x Delta 2510

## Compatibility:
Having wide compatibility is hard...

### Voron
Partial compatibility with voron trident and 2 gantries 
* Gantry must be flipped so there is more space under the xy joints
* Cablechains for X cant be used

### Monolith
**The flying gantry versions currently interfere with the part cooling fans, this may not mean Y loss but it can cause homing issues.**

| variant | compatibility status |
|---------------|------------------|
| printed 6mm belts | fully compatible |
| sheet metal 6mm belts | fully compatible |
| printed 9mm belts | "wings" interfere with the xy joints |
| sheet metal 9mm belts | "wings" interfere with the xy joints |

Note: The Y footprint of this toolhead is VERY small so you likely get extra travel. This means the Y travel can be smaller.

## Current TODO list:
* Belt clamps
* Ducts
* Wider monolith compatibility
* MGN12, the torsional stiffness is not needed because of the COM but why not :) 
