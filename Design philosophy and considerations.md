Hi! If you're here you probably want to learn more about the design and how/why it was made. I don't want to talk about those nerdy details in the readme so I made this!
If you have questions, feel free to reach out to me via discord!

### Form factor
This whole design started from wanting a toolhead with a super minimal Y footprint. I am working on a dual gantry printer where toolhead Y losses are doubled because there are well... 2 gantries. I didnt really find anything that had a super low Y footprint so I decided on a little scope creep as a treat. 

I am looking to go reasonably spicy with my printer (~80c) so I wanted good cooling, I considered dual 5015's but then I found tigers toolhead, takeoff, calamity and IROB. I had the idea of placing the hotend and fans under the X axis instead of in front like calamity does. This does make the toolhead quite tall and results in a relatively long bowden tube but the Y footprint is TINY. 2 of these toolheads next to eachother take up less Y space than a stealthburner (with cable chain), Of course there still need to be XY joints but those can be made small enough.

![image](https://github.com/user-attachments/assets/1d6f9516-790a-4afd-a3c5-7857401e8571)
![image](https://github.com/user-attachments/assets/88a10dbe-960a-4de5-8bf3-db4b17902362)



### cooling
As said before, 2 3628's were chosen for the task of cooling plastic in an 80c chamber. After looking around, I found that CBON's ducts were referenced a lot but they are meant more as area cooling ducts. They prioritize airflow over aiming the air, which is great for going very fast but I wanted to try something more focussed on the nozzle. I took the challenge of simulating the ducts in CFD, one of the first things I noticed is that I needed to either:
Make the ducts longer to give more space for the air direction to change, this idea is flawed because these axial fans dont have much static pressure. They dont like restrictive ducts.
or:
rotate the fans (this takes a bit of room in z but it allows me to make very short ducts. It also allows me to split up the airflow in an 'area cooling' and 'focussed cooling' part. The great thing about the tilt is that the focussed cooling has more length for the ducts to curve while simultaneously keeping the area cooling part short.
![image](https://github.com/user-attachments/assets/1457a6f7-a680-4e00-9b74-a8f87281f051)

There are a few features that I think stand out:
* there is a cone coming from the hub of the fans to remove the area of lower pressure air. this hopefully improves the flowrate a bit, but it also helps keep the ducts more rigid and printable. 
* The ducts themselves dont need any supports to be printed, and I am very proud of that. The probe mount options sadly may require supports. 



### 
