# A10 – Lead Screw Design

## Objective

Design and build a mechanically driven tensile tester capable of applying up to 2 kN axial tensile load with a controllable crosshead speed from 1 to 50 mm/min. Each team is responsible for the mechanical components outlined below. The system will provide consistent, well-aligned loading for polymers and light metals, suitable for instructional use and basic materials evaluation. Safety factor of 4, max deflection of 0.1 mm. 

## Leadscrew Design - Bryson Bare

I began by assuming steel with a yield strength of 310 MPa for the lead screws. This gave me a starting point for estimating the minimum diameter before selecting an actual screw. Assuming the two screws share the 2 kN load equally, each screw supports 1,000 N. I used axial stress and a safety factor of 4 to calculate a minimum diameter of approximately 4.05 mm. This represents the minimum diameter needed for axial strength under my assumed material properties and helped guide my selection of a commercially available lead screw.

<img width="504" height="505" alt="image" src="https://github.com/user-attachments/assets/d9c5213c-d492-41a8-83aa-91f9064ae8d5" />

After estimating the minimum diameter, I selected a 1/2"-10 lead screw and used its dimensions to calculate the required rotational speed and torque. With 10 threads per inch and a single-start thread, the screw advances 2.54 mm per revolution. Dividing the required crosshead speeds of 1–50 mm/min by this lead gave me a rotational speed range of approximately 0.39–19.68 rpm. Using the 1,000 N load per screw, an assumed friction coefficient of 0.2, and the dimensions shown in my calculations, I obtained an estimated torque of 1,695.831 N·mm per screw. These calculations connected the selected screw’s geometry to the motion and driving torque required for the tensile tester.

<img width="493" height="635" alt="image" src="https://github.com/user-attachments/assets/985b9e24-e9fd-48c6-a9ed-1509aeb12fcc" />


## Nut and Flange - Bryson Bare

Next, I researched McMaster-Carr’s recommended nuts and flanges for the lead screw I selected. I chose a 1/2"-10 flanged nut made from 932 bearing bronze to match the screw’s thread size. I calculated the number of engaged threads (N_t) by dividing the thread engagement length of 44.45 mm by the pitch of 2.54 mm, resulting in 17.5 engaged threads. I then used this value to calculate the thread bearing and bending stresses under the 1,000 N load per screw. Using a bronze yield strength of 124 MPa and a safety factor of 4, I calculated an allowable stress of 31 MPa. My calculated bearing stress of approximately 1.253 MPa and thread bending stress of approximately 4.229 MPa were below this value. Based on the dimensions and assumptions used in this analysis, the selected nut met the calculated thread-strength requirement.

<img width="506" height="652" alt="image" src="https://github.com/user-attachments/assets/aec8363f-69e3-4b17-90df-bd2e0191d209" />

Total time Bryson - 2.5 hours
 
## Crosshead Design - Nolan Brehaut
**Beam FBD**

The project parameters allowed us to design a crosshead with a lot of freedom. I did some research, and found that a 300mm crosshead (length) would work nicely. I then had to choose the material and thickness of the crosshead. I chose ASTM A36 steel for its high stiffness and a base width of 60mm. I then modeled the crosshead as a beam supported at both ends with a load in the center (as explained in lecture). I then found where the shear force = 0 (max moment location) and then found the max moment equation to equal PL/4. 

<img width="1920" height="643" alt="mail google" src="https://github.com/user-attachments/assets/ff0369f0-a51d-414a-96d5-4020d543c4a3" />


**Stress Analysis**

To perform a stress analysis, I did some algebra with the equations for stress due to bending on a beam, moment of inertia, and neutral axis to POI (c). I ended up with a derived equation for the minimum allowed height of the crosshead due to normal stress (due to bending) and plugged in the numbers to obtain a value of 15.49mm.

<img width="1920" height="378" alt="mail google" src="https://github.com/user-attachments/assets/2aafcde1-a95c-4905-bd66-49437cd33534" />


**Deflection Analysis**

To determine the minimum height of the crosshead in terms of deflection, I first took a cut of the left hand side of the beam, and determined the moment equation in terms of x. I then integrated twice to get the deflection and slope equation, and solved to finish my derivation of max deflection for the beam. Although this information is available online, I decided to derive it to get a better understanding for how these equations come to fruition. Using this equation, I derived an expression for the minimum height for the cross section of the crosshead, and got 22.41mm due to deflection. This would designate the true height since 22.41 is larger than the 15.49 due to stress. I rounded to 25 mm for ease during the CAD modeling and design process. 

<img width="1920" height="867" alt="mail google" src="https://github.com/user-attachments/assets/bed0d652-932f-46f2-afbc-1b9bf712d505" />


## Crosshead Sketch - Nolan Brehaut

For the handsketch, I only had one small decision to make. I made the holes cut for the leadscrew to pass through an inch in diameter just to ensure there was no contact with the lead screw and the wall of the crosshead. Everything else was determined by my previous math. 

<img width="3303" height="2754" alt="unnamed" src="https://github.com/user-attachments/assets/efebc4b6-420e-443c-8a88-498c418316d5" />


## Tabulating Cost - Nolan Brehaut

<img width="1500" height="700" alt="image" src="https://github.com/user-attachments/assets/f097cf5b-ed6b-48d6-b396-a570db9ad5d1" />

**Links :**

[Item #1](https://www.mcmaster.com/98940A305/)

[Item #2](https://www.mcmaster.com/97790A110/)

[Item #3](https://www.mcmaster.com/92316A540/)

[Item #4](https://www.mcmaster.com/47065T882-47065T752/)

Total time Nolan - 2.5 hours

## Parametric Modeling - Brandon Hudson 


## Lessons Learned 

Personally, I did the math for the crosshead. A lot of this was a repeat from previous assignments or from other classes. One thing I did learn however, was how to derive a deflection formula, instead of just searching it up online. One other thing that I learned when completing my part of this assignment was how extensive mcmaster-carr is. 
