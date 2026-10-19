# __Trinity-toolhead__

> [!NOTE]  
> This project lives in a user project in the monolith discord server.
Taking inspiration from Takeoff, Calamity, Tiger's toolhead, IROB and fiberstream, I came up with this: 
A small footprint unibody high performance toolhead. The goal for this toolhead is to prioritize performance while using fans on the toolhead. This toolhead is designed to push speed in hot chambers

* Made to DUEL! the tiny Y footprint makes it take up very little space for a dual gantry printers.
* Double 3628 fans deliver enough cooling even for hot chambers.
* The hotend is braced at the heatsink to increase stiffness
* Balanced center of mass (COM) for cleaner input shaper graphs and lower rail wear
* Single piece body to maximize stiffness and minimize weight.


<img width="3000" height="1400" alt="Untitled Project (17)" src="https://github.com/user-attachments/assets/debb5428-22b0-4adc-b62d-277d90ccb1e6" />
<p float="left">
<img width="335" height="670" alt="trinity 1.6 render side" src="https://github.com/user-attachments/assets/0219c608-78c5-42fd-bfe8-1a7bad4fbdd4" />
<img width="670" height="670" alt="trinity 1.6 render diagonal" src="https://github.com/user-attachments/assets/88672dc5-90ed-4025-99da-cc367ae0f013" />
</p>



## Compatibility:
<!--
### Voron
Partial compatibility with voron trident and voron 2 gantries 
* Gantry must be flipped
* Cablechains for X cant be used
-->


| Component | Supported Options & Variants | Notes |
| :--- | :--- | :--- |
| **Rails** | mgn12 | hiwin(clones) as well as airtac are tested |
| **Belts** | gates gt2 (and epdm) 6, 9 and 10mm | for 9mm belts, use the 10mm belts variant of the body |
| **Extruder** | sherpa mini v3 (by fysetc) | this is the only official option, support for others may be modded later but performance cant be guaranteed |
| **Hotend** | dragon ace volcano | this is the only official option, support for others may be modded later but performance cant be guaranteed |
| **Probes** | [Beacon](https://beacon3d.com/),  [cartographer](https://cartographer3d.com/), [Klicky00](https://github.com/DW-Tas/Klicky-00)  | an [adapter plate](https://github.com/WV-design/Trinity-toolhead/blob/main/Files%20(WIP)/extras/Trinity%20klicky00%20mounting%20plate%20by%20Prooda.STEP) is required for klicky00 |

## BOM:

| Amount | part | Note |
|-|-|-|
| 1 | Hotend | Recommended: <br /> [dragon ace volcano](https://trianglelab.net/products/dragon-ace%E2%84%A2-hotend?VariantsId=11350) |
| 1 | Extruder | Recommended: <br /> [Sherpa mini](https://www.fysetc.com/products/cnc-all-metal-sherpa-v3-extruder-light-weight-kit-36-moons) |
| 2 | 3628 fan | Recommended: [Delta FFB03612EHNYCL](https://www.digikey.com/en/products/detail/delta-electronics/FFB03612EHNYCL/6580720) <br /> Alternatively (a little less powerful) [FFB03612VN-00](https://www.digikey.com/en/products/detail/delta-electronics/FFB03612VN-00/24321211)|
| 1 | 2510 fan | Recommended: <br /> [delta ASB02505SHA-AY6B](https://www.digikey.com/en/products/detail/delta-electronics/ASB02505SHA-AY6B/7491489?s=N4IgTCBcDaIIIGUBCAGMBWF6EAk4Fo4BNANiRAF0BfIA) |
| 1 | monolith belt clamp | SLM: https://monolith-gantry-updates.zen3d.eu/monolith-slm-belt-clamps/ <br /> or CNC by dderg or LDO |
| 1 | PTFE Tube "micro" bowden  | 4x2x71mm |
| 4 | part cooling fan mounting | m3x35mm socket head | 
| 2 | part cooling fan mounting | m3x35 button head (these can be replaced with 2 more socket head screws)|
| 1 | K face mounting bolt | m3x30 button head|
| 4 | rail mounting bolts | m3x25 socket head|
| 2 | extruder mounting bolt | m3x16 button head|
| 2 | square nut | DIN 557 m3 |
| 8 | heat set insert | m3x4/5mm |
| 4 | hotend mounting bolts | m2.5x8mm |
| 2 | hotend fan mounting bolts | m2.5x14mm | 
| 2 | hotend fan heatset inserts | m2.5x4mm


### material choice:
> [!NOTE]  
> * Fiber filled filaments are preferred because of their stiffness
> * The apex clips should NOT be printed in a brittle material or be annealed! They can snap when inserting but will be fine once in place.

| Chamber Temp | Material | Notes |
| :--- | :--- | :--- |
| < 70C | ABS | is fine |
| < 100C | annealed PC-PBT/PET(NOT PETG!), or PC | look for a Tg of ~130C or higher, the rest is blended/impure and may creep<br><br>The armchair engineering and monolith discord servers have good info on annealing these materials |
| > 100C or for bonus points | annealed PPS/ultem | yes someone printed trinity in ultem 1010 |




> [!IMPORTANT]  
> make sure the ends of your belts are in good condition. If you re-use belts that have been used in another toolhead, be sure to double check them. This belt is a good example of a damaged one, the teeth are crushed so they wont grip the toolhead as well. <br />
![image](https://github.com/user-attachments/assets/69d3e6b4-8164-4774-8e41-9ad379f47fe9) <br />
> You need to check what belt clips fit best, this can differ per printer. You should use the **thickest** belt clamp that can still be inserted with one finger, friction is good but you dont want to damage the belt. There is a clip size test available in the "extras" folder. Also make sure the clips are in **all the way**. If the belts are not seated well the clips may not go in all the way. Below here are 2 examples of improperly installed clips. Make sure the legs of the clips are perfectly **parallel** and that all clips sit at the same height. <br /><br />
![image](https://github.com/user-attachments/assets/1f8e9bbc-02aa-41e8-a590-39a18656d3e8)
![image](https://github.com/user-attachments/assets/40e1e91b-7fc5-47d5-a53e-ca7e67595c07)


## Print Settings:
* Layer heights
  - body: <= 0.2mm
  - ducts: ideally ~0.12mm to make them smoother but anything from 0.1-0.24 should work
  - apex clips: ~0.1mm so the different thicknesses print properly
* Wall count: => 5
* Top/bottom layers: => 6
* Infill: this shouldnt really matter because of the walls and top layers but => 20% is nice for printing. My recommendation: 40% multi wall triangle infil 
* Print the parts **slowly**, strength and layer adhesion are important for the toolhead's performance. To achieve this, you can simply limit the flowrate in your slicer.
  

## Credits
Thanks to:
### Prooda, I'd consider him a co-designer at this point. He gave me lots of feedback and spent long nights refining the design.
### Martin, he's done a *lot* of work on modding trinity!

Apex, for your [awesome belt clips](https://github.com/ApexArray/ApexClips) and the insight!

Wayne, for the [monolith belt clamps](https://github.com/CloakedWayne/MISC/tree/main/Monolith_SLM_belt_clamps)

Hartk, for the [voron construct repository!](https://github.com/PrintersForAnts/Voron-Construct)

DK and Adeo, on the insights on the ducts!

And everyone who has shown support, given feedback or just showcased their builds, thank you!
