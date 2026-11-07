# A9 – Pulleys

## Objective
<p align="center">
<img width="295" height="100" alt="image" src="https://github.com/user-attachments/assets/6731cf00-c215-47f5-a1fd-b4fee9e61c5a" />
</p>

- Design a pulley system to transfer power between two parallel axes separated by a center distance of 4–6 inches.

- Pulleys shall have a diameter of 3 inches
  
- Operating speed must be between 1000 - 2000 rpm
  
- Belt tension 4-6 lbf
  
- Minimum safety factor of 3
  
- Polyurethane rubber 3.25 MPa (471 psi)

- Center distance of 4-6 inches 

## Selecting Suitable Belt
To select the most suitable belt, i had to make some calculations to find the diameter of the belt as well as the outer circumference of the belt. To find these values, I used the formulas found in the canvas module. I learned that one part of the belt is under way less tension than the other. I also learned that the max stress on the belt is calculated using the max force (higher force on the belt) rather than the initial torque applied. Here are all of my calculations:

<img width="1848" height="997" alt="0" src="https://github.com/user-attachments/assets/272983b8-5efe-4ce5-9495-9280702e2017" />


## Minimum Shaft Diameter
To calculate the minimum shaft diameter, I had to do some more calculations. I need the yield strength of 1060 hardened steel, which I found to be 70000psi:
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f90acfed-eab3-42d8-ad98-4ef0b12b2687" />
I derived the equation for net torque acting on the pulley by using T=F*d and summing the two forces with the radius of the pulley (1.5in). I then completed the rest of the calculations to determine the minimum shaft diameter as seen here:

<img width="1920" height="755" alt="0" src="https://github.com/user-attachments/assets/fa3389cc-d4e7-4100-af5a-1272513c5257" />


## Journal Bearing Design
After calculating for the Pressure, Velocity, and PV value, I checked the table for materials in the Machinery Handbook. I decided on Porous Bronze since it easily cleared the 3 safety factor being applied to the 8378 PV rating. Here are my calculations:

<img width="1920" height="563" alt="0" src="https://github.com/user-attachments/assets/992adef6-9f9e-4359-8e51-b9809088004e" />


## Frame Design
Using the given frame image, I decided upon a lightweight aluminum (6061-T6) because it is easy to machine with, lightweight, and can handle the forces being applied by the pulley. 

Given Frame:
<img width="870" height="356" alt="image" src="https://github.com/user-attachments/assets/85870c3c-e8e2-4bca-ae95-daacd8885168" />


## Lessons Learned
In this assignment, I learned a lot about pulleys and how they work. I also learned that there is one part of the belt that is way tighter than the other. This assignment also really helped nail in the concept of PV. This assignment took me roughly 2 hours to complete.
