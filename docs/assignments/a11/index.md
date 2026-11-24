# A11 – Motor Selection

## Objective
- Select a motor

- Design Motor Mounts

- Design a frame to support a crosshead stability and tensile load

- Select or design a Clamp Analysis and Design

- Provide complete CAD model of the engineered parts of the Tensile tester

- Deliver a Bill of Materials and Engineering cost

- 2kN load

- 1-50mm/min speed

- Safety Factor of 4 



<img width="322" height="463" alt="image" src="https://github.com/user-attachments/assets/48bbbcd4-5f04-4e49-a52f-db28c975c1af" />


## Motor Selection and Attachments - Bryson Bare

We selected the MOONS’ AM34HD2403-07 hybrid stepper motor because the tester must move slowly while pulling a high load. The stepper motor can provide controlled movement at low speeds, and this model has a listed holding torque of 9.4 N · m. We assumed that one motor would drive each lead screw, so each screw carries half of the tester's 2 kN load. The holding torque helped us identify a candidate, but we use the speed-torque curve to check the torque while the motor is running.


<img width="622" height="708" alt="image" src="https://github.com/user-attachments/assets/dd7c04f5-cc4f-497d-bdfc-0285c8ea0697" />




<img width="590" height="360" alt="image" src="https://github.com/user-attachments/assets/8913ad96-cb8d-4015-9826-f75897bd43c8" />



**Motor Mount Design** 


After selecting the motor, we needed to design a motor mount to hold it. We designed a four-bolt motor mount to attach the motor securely to the tester frame. We calculated the force on each bolt from the motor’s reaction torque, checked the plates' bearing stress, and found the minimum thickness needed to meet the allowable stress. Because the minimum thickness was so thin, we selected a 10mm plate for a more practical and rigid mount. I also had to account for the thickness of the top of the frame when choosing the bolt lengths that will hold the mount to the frame. I chose 20 mm because the mount is 10 mm thick and the frame is 10 mm thick.


<img width="612" height="812" alt="image" src="https://github.com/user-attachments/assets/f12ef486-26be-4728-a403-86b2163fbc6b" />


**Coupling Design**



We selected the McMaster-Carr 2764K425 coupler because its 14mm and ½ in bores match the motor shaft and the lead screws nominal diameter. This would connect the motor to the lead screw. The coupler is rated for 89 in*lbf, which is higher than our design torque. Its speed rating also exceeds the leads screws max speed. The flexible discs help accommodate any slight misalignment between the shafts. For a secure fit, the screw end will need to be a smooth section where it enters the coupling. 



<img width="607" height="683" alt="image" src="https://github.com/user-attachments/assets/6bbcb905-0706-462f-8f56-67b5d1c7ff39" />

Total Time Bryson - 5 hours

## Analyze and design a Frame - Nolan Brehaut

For analyzing the frame, I was tasked with running an FEA for the top of the frame and the vertical components of the frame, to ensure the frame will have very low deflections. 

**Top of the frame**

For the top of the frame, I loaded up the CAD assembly for our frame and started a new study. I then measured from the outside edge of the crosshead to the center of the leadscrew hole. 

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/25490138-3ea0-4ccd-bc12-bfdcb53eee5e" />

I used this measurement to determine where to put the 1kN forces on the top of the frame. I also added this distance to it

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/c432fa16-70db-4d42-b3aa-01feee6ea865" />

I then used this measurement to create a point on the surface of the beam that I could refer to when placing a force down. This did not work, which led me to having to sketch circles around the point. This also did not work, so I had to split the geometry for the face of the beam with the circles I sketched as seen here:


<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/bbe124e8-1aed-4e38-8d97-c99f936ab6a1" />

I then realized that after a 50/50 chance, I did this on the side that was underneath for the assembly, leading me to having to redo this again. After all of this which took around an hour to learn how to put a single force on this one specific location, I had this:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/72f8b92d-5b83-4fa7-8c1b-a9c92a0a7714" />

Mesh:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/7c4fa56a-3dd2-4b32-bd2d-608980d7ace1" />

I then realized although not stated in the canvas page, the analysis was supposed to be done for just the beam and not the whole frame and crosshead together. I created these forces and fixtures:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/23045c36-2740-4058-9dc5-502b9b4aabec" />

After applying a material and running the study, I was left with these results:

**Von Misses**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a4b9c51b-c14b-466d-9092-7d1f883e7586" />


**Deflection**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/dc121c31-0b86-4515-b860-2e7979039f15" />
  

**Safety Factor**

Safety factor was 7.7 everywhere.

This safety factor was well above the project's given 4 value, so I decided it was good to move on to the Side of the frame.


**Vertical Frame**

To check the vertical frame, I ensured that the frame could withstand the 1000N from the leadscrew, as well as the torque from the lead screw (calculated to be 16.6 N*m). Here are my forces and constraints:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/dea291c8-7c34-438f-b7dd-e715e8fc2764" />

I then ran the study and got these results:

**Von Misses**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/7d781d83-fcac-4f2e-8fdb-847dcf6091c1" />


**Deflection**

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/7f265017-b1c8-439f-b56a-2e165503775a" />


**Safety Factor**


I got back a calculated safety factor of 12. This was way above the safety factor of 4, so I decided to deduct that this frame was built strong enough to not need any changes to the overall design. 

Total time Nolan: 2 hours


## Design Floating Bearing Mount -  Brandon Hudson


I first started designing the motor mount with the dimensions Bryson came up with in the math above. Below is the sketch of the motor mount. 

<img width="445" height="332" alt="image" src="https://github.com/user-attachments/assets/a5fd0f9f-9489-4a3c-95b6-74f3e2609dce" />

After doing the sketch I completed the extrude which was a total of 10mm. I then created the 4 holes on the mount and dimensioned them to the correct dimensions given to me by Bryson.  Below is the motor mount after this extrude and the holes inserted. 

<img width="461" height="311" alt="image" src="https://github.com/user-attachments/assets/50f31fac-02d3-44b2-a03a-22269f24c407" />

After completing the extrude and holes I finished up the motor mount. Below is the final product of the motor mount. 

<img width="428" height="300" alt="image" src="https://github.com/user-attachments/assets/ff69e094-7401-4fe0-894f-869ba91041e9" />


I then moved onto the assembly by downloading the couplings, motor, and screws needed to fully assemble the motor and frame. I got all the parts needed and began assembling the finished product. Below is the final assembly. 


<img width="215" height="251" alt="image" src="https://github.com/user-attachments/assets/3797d40c-eda7-4453-83b2-ba5d8ac4d48f" />


<img width="202" height="222" alt="image" src="https://github.com/user-attachments/assets/467bdf51-4b73-4b65-8bc8-9cfbb7d14d6a" />


## Bill of Materials and Labor costs - Brandon Hudson

| Item # | Quantity | Name | Cost/item | Cost | Link |
|:---|:---:|:---|---:|---:|:---|
| AM34HD2403-07 | 2 | Hybrid Stepper Motor | $198.00 | $396.00 | [MOONS' - AM34HD2403-07](https://www.moonsindustries.com/p/am-series-standard-hybrid-stepper-motors/am34hd2403-07-000004611110010745) |
| 2764K425 | 2 | Shaft Coupling | $118.34 | $236.68 | [McMaster-Carr](https://www.mcmaster.com/2764K425/) |
| 91274A141 | 1 pack (50) | Socket Head Screw | $10.63 / 50 | $10.63 | [McMaster-Carr](https://www.mcmaster.com/91274A141/) |
| 98940A305 | 2 | Lead Screw | $28.64 | $54.56 | [McMaster-Carr](https://www.mcmaster.com/98940A305/) |
| 97790A110 | 2 | Flange Nut | $178.60 | $357.20 | [McMaster-Carr](https://www.mcmaster.com/97790A110/) |
| 92316A540 | 4 | Socket Head Screw | $10.02 / 50 | $10.02 | [McMaster-Carr](https://www.mcmaster.com/92316A540/) |
| 47065T882 | 1 | Frame | $125.63 | $125.63 | [McMaster-Carr](https://www.mcmaster.com/47065T882-47065T752/) |
| **Total Cost** | | | | **$1,190.72** | |


Total time Brandon - 8 hours


## Lessons Learned

One lesson I learned throughout my portion of this assignment was that there can be a lot of bigger steps that are all new to you, just to complete something very small. It took me roughly half my total time for my part of this assignment just to learn how to create a point load in a specific spot in solidworks. The one good thing to come from that, is that I will not forget how to replicate this for a long time.  


[Google Folder with CAD](https://drive.google.com/drive/folders/16NzgxDtks0Jcl7XMD67j7Hv-oHWpTYXf?usp=sharing)
