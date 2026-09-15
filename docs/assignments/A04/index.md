# A4 – [Motor Mount]

## Objective
Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations) Follow Appendix B for the initial approach to set up the design analysis.

<p align="center">
<img width="123" height="99" alt="image" src="https://github.com/user-attachments/assets/7a48d8a4-fbe3-4038-b18d-494e47cd3ee3" />
</p>

## Feature 1 
For feature 1,I first started off by sketching a FBD of the feature. As shown in the supplied images on the canvas page, the motor mount separates at the connection of the two parts, with feature 1 getting the intersection as part of it's dimensions.  - _Appendix A_

<img width="800" height="800" alt="1" src="https://github.com/user-attachments/assets/c8ee679d-9ce9-4902-9790-34429331e3ce" />

I realized that the fixture on the right side of the base created a canteliver beam type of situation for this base. This would allow for us to use the formulas for beam defelctions to relate to the given parameters.


I then calculated the the external forces to relate the moments about the right side of the base to the height of the base. Next, I designed the height based off of my yield strength. After doing research inside of the [following](https://www.specialchem.com/plastics/guide/acrylonitrile-butadiene-styrene-abs-plastic) website, I learned that the average ABS yield strength is between 29.6-48 MPa. I decided to chose 35 MPa as it was a multiple of 5 and was very close to the middle of the two. After using the stress, I, and c equations from lecture, I got that the minimum height required in terms of the yield strength must be 5.15mm. Next, I did the same process using the given 0.30 mm max deflection. From this math I got that the minimum height had to be 9.5mm. Since this is a larger value than the previous _minimum_ value I calculated, this was the value that I was left with. 

**Here is my math for feature 1:**

<img width="1000" height="800" alt="1" src="https://github.com/user-attachments/assets/74746dfc-0334-44f0-a4a9-37cc2c5b6b8b" />

## Feature 2 
After doing research within past student's A4 portfolio pages, I learned that rotating the axis essentially and allowing for the height to be the thickness of the backplate let me use the same numerical value for the moment that I had calculated in the previous feature. I also had to calculate the height (now base) with some simple addition/subtraction, since the intersection between the 2 features was accounted for in feature 1's FBD. Here is the FBD for feature 2:

<img width="800" height="800" alt="1" src="https://github.com/user-attachments/assets/99a5f773-633a-4ee2-85c6-bb0bd5250ff4" />

After making the FBD, I solved for external forces and found the moments to be 285N*mm after plugging in our previously determined height. Next, I w.r.t the yield strength once again and got 1.724mm. My next step was to solve w.r.t deflection, but as the assignment states, the plate is rigid against the wall. This would result in a height of 0. Rounding the 1.724 to 1.8 mm, I had my thickness of feature 2. 

**Here is my math for feature 2:**

<img width="1000" height="800" alt="1" src="https://github.com/user-attachments/assets/ce8d6e5e-a123-4238-bc77-ab8156da75d8" />

## Isometric Sketch
<img width="3024" height="4032" alt="unnamed" src="https://github.com/user-attachments/assets/8c99f613-85ab-4798-8198-792a15dfcbf8" />

## Parametric CAD Model

To start the CAD model, I first extruded a sketch off of the front plane to be the motor mount's base. Each side was 30mm, which meant that I had made the width of the sketch 30mm, as well as the depth of the extrude. I made the height of the sketch the previously calculated 9.5mm.

<img width="1920" height="1200" alt="1" src="https://github.com/user-attachments/assets/18d292c5-f981-43d0-9c07-69cbbabadf89" />

Next, I made another simple sketch off of the top of this extrude, I then extruded the sketch upwards by 85mm, as previously calculated.

<img width="1920" height="1200" alt="1" src="https://github.com/user-attachments/assets/3442ecdb-b0a4-4209-a965-86f64a7d4b88" />

Next, I cut a hole out of the top surface of the motor mount. This was done by selecting Extrude cut, and then creating a sketch of the hole. I used smart dimensions to ensure that the hole was the correct diameter (later changed from 22 mm to 18) to ensure a correct fit for the part. This dimension was found from the image under _Appendix B_ . The purpose of this hole is to allow the base of the motor to sit flush with the base of the motor mount. 

<img width="1920" height="1200" alt="1" src="https://github.com/user-attachments/assets/f23e77c9-a103-4f30-bfa1-50c9d8c45179" />

Following this hole, I created another hole that would go through the whole base of the motor mount this time. This hole was cut to allow for the shaft of the motor to go through the base, as seen in the project's supplied image (at the top of this page). I used the same techniques for this hole with smart dimensions. 

<img width="1920" height="1200" alt="1" src="https://github.com/user-attachments/assets/19a58324-6cfc-405a-9aae-78e86a6574d5" />

Lastly, 3.4mm holes were cut around a centered 22mm radius on the base of the motor mount. This was to account for the mounting process of the motor onto the mount, by the use of M3 bolts. The 3.4mm size was given to us on the canvas page. Here you can see my constraining of the holes, to ensure they are all centered on the base as well as inside the 22mm circle. The circle and the guidelines were all deleted before cutting through the top of the mount's base. These measurements can also be seen in _Appendix B_ .

<img width="1920" height="1200" alt="1" src="https://github.com/user-attachments/assets/eea14ff8-7c5f-42ab-862c-9e5eb02ef6d5" />

Here is my finished motor mount:

<img width="1920" height="1200" alt="1" src="https://github.com/user-attachments/assets/3fb1b854-a4f1-483e-9eba-b3b743a50a0a" />






## Reflection 
This project took me just about 4.5 hours to complete. I learned more about CAD modeling using solid works, as well as learning about cantilever beams. 


[Google Folder with CAD Files](https://drive.google.com/drive/folders/1-wBt3nmzCxCIUVWS0UIrUuQ9umav4i4K?usp=drive_link)



_**Appendix A**_

<img width="380" height="194" alt="image" src="https://github.com/user-attachments/assets/98e9a80b-886e-4794-818c-a10f0139201b" />

_**Appendix B**_

<img width="733" height="281" alt="image" src="https://github.com/user-attachments/assets/ed0ab911-aff6-4ff6-a95a-8da90d9f8f7c" />

