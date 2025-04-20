# __Trinity-toolhead__

I took inspiration from Takeoff, Calamity, Tiger's toolhead, IROB and fiberstream, and came up with this: 
A small footprint unibody high performance toolhead option.

![Untitled Project (16)](https://github.com/user-attachments/assets/cbb489eb-387c-4980-9744-d056e0c275b1)

## This is currently untested, I am still working on it. I would love your feedback! Discord: gerbz_ 

* The body is a single print to maximize weight, strength and stiffness.
* The hotend is supported at the bottom of the heatsink to increase stiffness.
* Double 3628 fans deliver enough cooling even for hot chambers.
* Made to DUEL! the Y footprint fits within a sherpa mini.
* Relatively light weight, estimated ~400g.
* Good COM


## Compatibility:

Note: The Y footprint of this toolhead is VERY small so you likely get extra travel. This means the Y travel, and thus the printer as a whole can be smaller.

### Voron
Partial compatibility with voron trident and 2 gantries 
* Gantry must be flipped so there is more space under the xy joints
* Cablechains for X cant be used

### Monolith
currently only mgn12 is supported
| variant | compatibility status |
|---------------|------------------|
| printed 6mm belts | fully compatible |
| sheet metal 6mm belts | fully compatible |
| printed 9mm belts | fully compatible |
| sheet metal 9mm belts | fully compatible |
| > 9mm belts | not supported |



## Recommended parts:
* 1x Fystec sherpa mini v3
* ~~bad~~ dragon ace volcano
* 2x Delta 3628
* 1x Delta 2510
### GT2 belts only for now, gt3 is thicker and needs way more tension. 


## Print Settings:
* Layer height: anything between 0.04-0.2mm should be fine
* Wall count: 6- only walls
* Top/bottom layers: ~ 5
* Infill: shouldnt really matter because of the walls and top layers
* Counterbore holes partially bridged is recommended
* Print it **slowly**, strength and layer adhesion are important for the toolhead's performance. 


## materials:
Fiber filled filaments are preferred because of the increase in stiffness 
* < 70C ABS 
* < 100C PC-PBT
* PC (look for a Tg of ~130C or higher, the rest is blended/impure)
* PET (annealed)
* PPS (annealed) (also what chamber temp are you planning to go for?? poor fans...)




## Credits
Thanks to:
Apex, for your [awesome belt clips](https://github.com/ApexArray/ApexClips) and the insight!

Wayne, for the [monolith belt clamps](https://github.com/CloakedWayne/MISC/tree/main/Monolith_SLM_belt_clamps)

Annex, for the [extruder design!](https://github.com/Annex-Engineering/Sherpa_Mini-Extruder)

Hartk, for the [voron construct repository!](https://github.com/PrintersForAnts/Voron-Construct)

DK and Adeo, on the insights on the ducts!

Barthini and Caza, for feedback on the design

