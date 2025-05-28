# __Trinity-toolhead__

Taking inspiration from Takeoff, Calamity, Tiger's toolhead, IROB and fiberstream, I came up with this: 
A small footprint unibody high performance toolhead.

![Untitled Project (5)](https://github.com/user-attachments/assets/e66abe7d-150d-415a-bc50-0d7e416bb486)

> [!NOTE]  
> This is currently being tested, I am still working on it and would love your feedback!
>
> an update is coming soon, I'd hold off on printing for a bit. this message will be gone after the update.
>
> This project lives in a user project in the monolith discord server.


* Made to DUEL! the Y footprint fits within a sherpa mini.
* Double 3628 fans deliver enough cooling even for hot chambers.
* The hotend is braced at the bottom of the heatsink to increase stiffness.
* Good COM (between the balls on the linear rails)
* Unibody to minimize bending and weight.


## Compatibility:

> [!WARNING]  
> Double Check compatibility for yourself, the cad has changed quite a lot so I may have missed compatibility issues.

<!--
### Voron
Partial compatibility with voron trident and voron 2 gantries 
* Gantry must be flipped
* Cablechains for X cant be used
-->

### Monolith
Compatible with 6 and 9mm belts, mgn9 and mgn12 (with the monolith SLM belt clamp

### GT2 belts only for now as gt3 needs a lot higher tension. 

## BOM:

| Amount | part | Note |
|-|-|-|
| 1 | Hotend | Recommended: <br /> [dragon ace volcano](https://trianglelab.net/products/dragon-ace%E2%84%A2-hotend?VariantsId=11350) |
| 1 | Extruder | Recommended: <br /> Sherpa mini |
| 2 | 3628 fan | Recommended: <br /> [Delta FFB03612EHNYCL](https://www.digikey.com/en/products/detail/delta-electronics/FFB03612EHNYCL/6580720) move the most air but are the loudest <br /> [Delta FFB03612EHN-BGA](https://www.digikey.com/en/products/detail/delta-electronics/FFB03612EHN-BGA/3283582?s=N4IgTCBcDaIGJwEIAYDMA2AjGAogCQDkBaRAcQEEQBdAXyA) are more quiet |
| 1 | 2510 fan | Recommended: <br /> [delta ASB02505SHA-AY6B](https://www.digikey.com/en/products/detail/delta-electronics/ASB02505SHA-AY6B/7491489?s=N4IgTCBcDaIIIGUBCAGMBWF6EAk4Fo4BNANiRAF0BfIA) |
| 1 | SLM monolith belt clamp | Only required for the MGN12 version |
| 4 | rail mounting bolts | m3x20 |
| 4 | m2.5x8mm | hotend mounting bolts |
| 8 | m3x35mm | part cooling fan mounting |
| 4 | m2.5x12 | hotend fan mounting
| 11 | m3 heat set insert | 4 or 5mm
| 4 | m2.5 heat set insert | for the hotend fan



## Print Settings:
* Layer height: 0.2mm for the body and ducts, 0.1mm for the apex clips and belt clamp. 
* Wall count: 6- only walls
* Top/bottom layers: ~ 6
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
> [!IMPORTANT]  
> make sure the ends of your belts are in good condition. If you re-use belts that have been used in another toolhead, be sure to double check them. This belt is a good example of a damaged one, the teeth are crushed so they wont grip the toolhead as well. <br />
![image](https://github.com/user-attachments/assets/c6c9eb85-05e9-4c4f-a314-961a93c88949) <br />
> You need to check what belt clips fit best, this can differ per printer. You should use the **biggest** belt clamp that can still be inserted with one finger. There is a clip size test available. Also make sure the clips are in **all the way**. If the belts are not seated well the clips may not go in all the way. Below here are 2 examples of improperly installed clips. Make sure the legs of the clips are perfectly **parallel** and that all clips sit at the same height. <br /><br />
![image](https://github.com/user-attachments/assets/1f8e9bbc-02aa-41e8-a590-39a18656d3e8)
![image](https://github.com/user-attachments/assets/40e1e91b-7fc5-47d5-a53e-ca7e67595c07)




## Credits
Thanks to:
Prooda, I'd consider him a co-designer at this point. he gave me lots of feedback and spent long nights refining the design.

Apex, for your [awesome belt clips](https://github.com/ApexArray/ApexClips) and the insight!

Wayne, for the [monolith belt clamps](https://github.com/CloakedWayne/MISC/tree/main/Monolith_SLM_belt_clamps)

Hartk, for the [voron construct repository!](https://github.com/PrintersForAnts/Voron-Construct)

DK and Adeo, on the insights on the ducts!

Barthini, Caza and Prooda for feedback on the design

