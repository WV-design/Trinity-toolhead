## Heads up, read this page before printing!
Trinity is too tall for most belt tensioners, therefore Prooda developed a new one. This can be found in the "extras" section

### Print settings:
* Layer height: anything between 0.04-0.2mm should be fine. Consider a smaller (~0.12mm) layer height for the ducts
* Wall count: ~6-solid(only walls).
* Top/bottom layers: => 5
* Infill: doesn't really matter because of the walls and top layers but ~25% helps with internal overhangs.
* Print it slowly, strength and layer adhesion are important for the toolhead's performance. The easiest way to do this is to limit the flowrate in the slicer.

### material choice:
Fiber filled filaments are preferred because of the increase in stiffness 
* < 70C ABS 
* < 100C PC-PBT
* PC (look for a Tg of ~130C or higher, the rest is blended/impure and may creep)
* PET (annealed)
* PPS (annealed) (also what chamber temp are you planning to go for?? poor fans...)

### selection single/multi color
I designed a "logo cutout" piece so you can choose how to print the logo. Options include:
- multi color. the file includes inset edges on the front face, so the slicer should be able to easily fill the faces with colors.
- single color without logo, this is the easiest, you simply delete the logo cutout before printing.
- single color with inset logo, for this option you need to do some slicer tricks. You can use the "logo cutout" as a negative body to cut into the main body. It's explained in [this video](https://www.youtube.com/watch?v=_e7CY2rMzgA)
