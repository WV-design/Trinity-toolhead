Hi! If you're here you probably want to learn more about the design and how/why it was made. I don't want to talk about those nerdy details in the readme so I made this!
If you have questions, feel free to reach out to me via discord!

### Form factor
This whole design started from wanting a toolhead with a super minimal Y footprint. I am working on a dual gantry printer where toolhead Y losses are doubled because there are well... 2 gantries. I didnt really find anything that had a super low Y footprint so I decided on a little scope creep as a treat. 

I am looking to go reasonably spicy with my printer's chamber (~80c) so I wanted good cooling, more on this in the *cooilng* section. I considered dual 5015 blower fans, but then I found tigers toolhead, takeoff, calamity and IROB, which all used 3628 axial fans to great effect. Then I had the idea of placing the hotend and fans under the X axis instead of in front like calamity does. This results in a toolhead that is super compact in the Y direction, and can balance the mass of the components very well. The result is a toolhead with extra travel in Y, great cooling, and a well placed center of mass (COM). It does, however result in significant Z loss because the toolhead is quite tall. 2 of these toolheads next to eachother take up a similar Y footprint compared to a stealthburner (with cable chain).

![image](https://github.com/user-attachments/assets/1d6f9516-790a-4afd-a3c5-7857401e8571)
![image](https://github.com/user-attachments/assets/88a10dbe-960a-4de5-8bf3-db4b17902362)


### cooling
As said before, 2 3628's were chosen for the task of cooling plastic below its glass transition temperature (Tg) as fast as possible. This is difficult because the chamber's temperature can be just a few degrees below the material's leading to poor heat exchange because of the low temperature delta. After looking around, I found that CBON's ducts were referenced a lot but they are meant more as area cooling ducts. They prioritize airflow over aiming the air, which is great for going very fast but I wanted to try something more focused. I took the challenge of simulating the ducts in CFD, one of the first things I noticed is that I needed to either:
* Make the ducts longer to give more space for the air direction to change, this idea is flawed because these axial fans dont have much static pressure. They don't like back pressure so the ducts needed to be unrestrictive.
or:
* rotate the fans slightly (this takes a bit of room in z but it allows me to make very short ducts. It also allows me to split up the airflow in an 'area cooling' and 'focused cooling' part. The great thing about the tilt is that the focused cooling has more length for the ducts to curve while simultaneously keeping the area cooling part short.
![image](https://github.com/user-attachments/assets/1457a6f7-a680-4e00-9b74-a8f87281f051)

There are a few features that I think stand out:
* there is a cone coming from the hub of the fans to remove the area of lower pressure air behind the motor hub. This aims to lower turbulence and improve the flow rate a bit, but it also helps keep the ducts more rigid and printable. 
* The ducts themselves don't need any supports to be printed, and I am very proud of that. The probe mount options sadly may require supports. 


### Compatiblity
With the strict requirements of good COM, print-ability, stiffness, and keeping a low footprint, the task of adding compatibility gets exponentially more difficult. the toolhead body needs to change for every variant which adds up fast. Just having 6 and 9/10mm belt, mgn9 and 12 rail, and Sherpa mini and orbiter extruder support would mean I need to make 2*2*2=8 versions of the toolhead body. This gets unsustainable with slight changes or improving the CAD. At one point the project got so overwhelming that I did not want to touch it anymore so change was needed.
First, plans for supporting a filament cutter, or filament sensor were quickly scrapped. The same was done with the mgn9 rail variant, because monolith is designed for a mgn12 rail so thats what most users opt for. On top of that, the orbiter variants seemed to perform poorly with a double Y peak on the input shaper graphs. This likely meant that the extruder was "nodding" around the z axis despite the built in support for the motor that sticks out. Because of this, orbiter support was dropped. 
