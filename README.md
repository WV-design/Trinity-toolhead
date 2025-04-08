# __Trinity-toolhead__
A small footprint monolithic high performance toolhead option.
![Untitled Project (12)](https://github.com/user-attachments/assets/a59dac44-85e1-497b-a686-303b4712fa22)



I took inspiration from Takeoff, Calamity, Tiger's toolhead and IROB, and came up with this.

## This is currently untested, I am still working on it. I would love your feedback!
Discord: gerbz_

* The body is a single print for maximum stiffness.
* The hotend is supported at the bottom of the heatsink to increase stiffness
* Couble 3628 fans deliver enough cooling for hot chambers
* Optimised for dual gantry printers, the toolhead itself has a smaller Y footprint than the sherpa mini.
* Light weight, estimated ~360g
* The COM is absolutely on point!
  
![image](https://github.com/user-attachments/assets/4b7fee9b-9277-448e-b6ef-d20bfc20db1b)

## Recommended parts:
* 1x Fystec sherpa mini v3
* ~~bad~~ dragon ace volcano
* 2x Delta 3628
* 1x Delta 2510

## Monolith compatibility:
**The flying gantry versions currently interfere with the part cooling fans, this may not mean Y loss but it can cause homing issues.**

| variant | compatibility status |
|---------------|------------------|
| printed 6mm belts 2wd | fully compatible |
| printed 6mm belts 4wd | fully compatible |
| printed 9mm belts 2wd | "wings interfere" with the xy joints |
| printed 9mm belts 4wd | "wings" interfere with the xy joints |
| sheet metal 6mm belts 2wd | fully compatible |
| sheet metal 6mm belts 4wd | fully compatible |
| sheet metal 9mm belts 2wd | "wings" interfere with the xy joints |
| sheet metal 9mm belts 4wd | "wings" interfere with the xy joints |


## Current TODO list:
* Forgot to do the K face mounting
* Ducts
* Belt clamps
* Wider monolith compatibility
* MGN12, the torsional stiffness is not needed because of the COM but why not :) 
