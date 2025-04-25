# __Trinity-toolhead__

Taking inspiration from Takeoff, Calamity, Tiger's toolhead, IROB and fiberstream, I came up with this: 
A small footprint unibody high performance toolhead.

![Untitled Project (16)](https://github.com/user-attachments/assets/cbb489eb-387c-4980-9744-d056e0c275b1)

> [!NOTE]  
> This is currently untested, I am still working on it. I would love your feedback! Discord: gerbz_ 

* Made to DUEL! the Y footprint fits within a sherpa mini.
* Double 3628 fans deliver enough cooling even for hot chambers.
* Unibody to maximize strength and stiffness with minimal weight.
* The hotend is braced at the bottom of the heatsink to increase stiffness.
* Relatively light weight, estimated ~400g.
* Good COM


## Compatibility:

> [!WARNING]  
> Double Check compatibility for yourself, the cad has changed quite a lot so I may have missed compatibility issues.

### Voron
Partial compatibility with voron trident and 2 gantries 
* Gantry must be flipped so there is more space under the xy joints
* Cablechains for X cant be used

### Monolith
Compatible up to 9mm belts

## BOM:

### GT2 belts only for now as gt3 needs a lot higher tension. 

| Amount | part | Note |
|-|-|-|
| 1 | Hotend | Recommended: <br /> [dragon ace volcano](https://trianglelab.net/products/dragon-ace%E2%84%A2-hotend?VariantsId=11350) |
| 1 | Extruder | Recommended: <br /> Sherpa mini |
| 2 | 3628 fan | Recommended: <br /> [Delta FFB03612EHNYCL](https://www.digikey.com/en/products/detail/delta-electronics/FFB03612EHNYCL/6580720) move the most air but are the loudest <br /> [Delta FFB03612EHN-BGA](https://www.digikey.com/en/products/detail/delta-electronics/FFB03612EHN-BGA/3283582?s=N4IgTCBcDaIGJwEIAYDMA2AjGAogCQDkBaRAcQEEQBdAXyA) are more quiet |
| 1 | 2510 fan | Recommended: <br /> [delta ASB02505SHA-AY6B](https://www.digikey.com/en/products/detail/delta-electronics/ASB02505SHA-AY6B/7491489?s=N4IgTCBcDaIIIGUBCAGMBWF6EAk4Fo4BNANiRAF0BfIA) |
| 1 | SLM monolith belt clamp | **OPTIONAL** |
| 4 | rail mounting bolts | m3x20 (mgn12 version |
| 4 | m2.5x8mm | hotend mounting bolts |
| 8 | m3x35mm | part cooling fan mounting |
| 4 | m2.5x12 | hotend fan mounting
| 11 | m3 heat set insert | 4 or 5mm
| 4 | m2.5 heat set insert | for the hotend fan



## Print Settings:
* Layer height: anything between 0.2mm is tested, smaller should also be fine
* Wall count: 6- only walls
* Top/bottom layers: ~ 5
* Infill: shouldnt really matter because of the walls and top layers
* Counterbore holes partially bridged is recommended
* Print it **slowly**, strength and layer adhesion are important for the toolhead's performance. 


### materials:
> [!TIP]
> Fiber filled filaments are preferred because of the increase in stiffness 

* < 70C ABS 
* < 100C PC-PBT
* PC (look for a Tg of ~130C or higher, the rest is blended/impure)
* PET (annealed)
* PPS (annealed) (also what chamber temp are you planning to go for?? poor fans...)

## assembly (will come after the cad is more stable)


## Credits
Thanks to:
Apex, for your [awesome belt clips](https://github.com/ApexArray/ApexClips) and the insight!

Wayne, for the [monolith belt clamps](https://github.com/CloakedWayne/MISC/tree/main/Monolith_SLM_belt_clamps)

Annex, for the [extruder design!](https://github.com/Annex-Engineering/Sherpa_Mini-Extruder)

Hartk, for the [voron construct repository!](https://github.com/PrintersForAnts/Voron-Construct)

DK and Adeo, on the insights on the ducts!

Barthini, Caza and Prooda for feedback on the design

