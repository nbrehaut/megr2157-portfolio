# A4 – [Motor Mount]

## Objective
Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations) Follow Appendix B for the initial approach to set up the design analysis.

<p align="center">
<img width="123" height="99" alt="image" src="https://github.com/user-attachments/assets/7a48d8a4-fbe3-4038-b18d-494e47cd3ee3" />
</p>

## Feature 1 
For feature 1,I first started off by sketching a FBD of the feature. As shown in the supplied images on the canvas page, the motor mount separates at the connection of the two parts, with feature 1 getting the intersection as part of it's dimensions. 

<img width="800" height="800" alt="1" src="https://github.com/user-attachments/assets/c8ee679d-9ce9-4902-9790-34429331e3ce" />

I then calculated the the external forces to relate the moments about the right side of the base to the height of the base. Next, I designed the height based off of my yield strength. After doing research inside of the [following]([url](https://www.specialchem.com/plastics/guide/acrylonitrile-butadiene-styrene-abs-plastic)) website, I learned that the average ABS yield strength is between 29.6-48 MPa. I decided to chose 35 MPa as it was a multiple of 5 and was very close to the middle of the two. After using the stress, I, and c equations from lecture, I got that the minimum height required in terms of the yield strength must be 5.15mm. Next, I did the same process using the given 0.30 mm max deflection. From this math I got that the minimum height had to be 9.5mm. Since this is a larger value than the previous _minimum_ value I calculated, this was the value that I was left with. 

**Here is my math for feature 1:**

<img width="1000" height="800" alt="1" src="https://github.com/user-attachments/assets/74746dfc-0334-44f0-a4a9-37cc2c5b6b8b" />

## Feature 2 
After doing research within past student's A4 portfolio pages, I learned that rotating the axis essentially and allowing for the height to be the thickness of the backplate let me use the same numerical value for the moment that I had calculated in the previous feature. I also had to calculate the height (now base) with some simple addition/subtraction, since the intersection between the 2 features was accounted for in feature 1's FBD. Here is the FBD for feature 2:

<img width="800" height="800" alt="1" src="https://github.com/user-attachments/assets/99a5f773-633a-4ee2-85c6-bb0bd5250ff4" />

After making the FBD, I solved for external forces and found the moments to be 285N*mm after plugging in our previously determined height. Next, I w.r.t the yield strength once again and got 1.724mm. My next step was to solve w.r.t deflection, but as the assignment states, the plate is rigid against the wall. This would result in a height of 0. Rounding the 1.724 to 1.8 mm, I had my thickness of feature 2. 

**Here is my math for feature 2:**

<img width="1000" height="800" alt="1" src="https://github.com/user-attachments/assets/ce8d6e5e-a123-4238-bc77-ab8156da75d8" />

## Isometric Sketch

## Parametric CAD Model

## Lessons Learned 


_**Appendix A**_


_**Appendix B**_


