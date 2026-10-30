# A8 – Gear Box Design

## Objective
- Design a gearbox that can be taken apart and put back together
- Determine specifications for both input and output shafts
- Design journal bearings to support the shafts
- Create and hand sketch a gearbox housing
- Create a CAD model of the final design

**Specifications**
- Gear ratio 24:9
- Output gear torque = 1.25 in-lbf @ 1100rpm 
- Input shaft to be .125 in , length of 1 inch 
- Output shaft to be .25 in , length of 1 inch 
- Shafts are press fit through the hubs of the gears
- Input is coming from the pinion gear

## Design the Shafts


**Input Shaft**
My first step in designing the input shaft was to calculate the rpm and the torque that was being applied to it due to the given output shaft values. This was done using the given gear ratio of 24:9. I then drew out the FBD of the input shaft, and calculated for the max allowed shear stress. The c value was calculated by using the radius of the shaft, because it is the distance from the outside edge of the shaft to the center. The value I obtained for max shear stress (1222.31 psi) is less than the 4000 that I found in the machinery handbook. Here is all of my math for the input shaft:

<img width="3320" height="1038" alt="unnamed" src="https://github.com/user-attachments/assets/c00e3510-d156-404a-9ad6-9173e82d69ca" />




**Output Shaft**
For the output shaft, I simply drew the FBD, wrote down the values that were given, and plugged in the values to the previously derived equation that I had made from the input shaft. My max shear stress was roughly 407 psi, which is way below the 8500 psi written in the handbook. This meant that both of the given diameters proved to be sufficient. Here are my calculations and FBD for the output shaft:

<img width="3292" height="675" alt="unnamed" src="https://github.com/user-attachments/assets/a3287172-164f-4cce-bd18-dd7991e44a76" />




## Journal Bearings
To start off designing the journal bearings, I had to do some research on how they worked. I learned that the journal bearing serves an important purpose of allowing for the shaft to rotate (in this case using a running sliding fit) whilst staying stationary with respect to the housing of the gearbox. I also learned that lubricant (typically oil) is applied  to the contact surface between the bearing and the shaft to mitigate friction.  

**Size and Length**
For the size and length, I did some research and found that a standard length for both a journal bearing with a 0.25 inch and a 0.125 inch inner diameter is 0.25 inch. I went on the supplied websites for the gears and found that the pitch is 48 and the pressure angle is 20 degrees for both. It also gives the gear pitch diameter for both, which we need for our force calculation. 

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/07f45d36-cb94-440a-b311-1cd6b0f8d4d9" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/e1820640-ce8f-4980-82ee-f47f82377f2a" />

I derived for the equation for force from the equation of torque. I then found the velocity and Pressure for each bearing. Multiplying these together gave me the pressure-velocity rating needed for each bearing. Here are my calculations:


<img width="3816" height="2138" alt="unnamed" src="https://github.com/user-attachments/assets/07255d1d-9c93-4a29-8956-0ef16d1dd009" />



**Thickness**
Using my found pressure-velocity ratings, I found a material off of McMaster-Carr that would be at a PV max of 10 ksi. This gave me the "Moisture-Resistant Dry-Running Rulon LR Sleeve Bearing". I selected two that were 1/4 inch long, with one being for a 1/4' inner diameter, and one being for 1/8" inner diameter.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/228a52c0-cf5d-43a9-a2d5-7d898dff1063" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/2a68da91-039f-4816-bc54-f0ced89a1c29" />

These bearings allow for a 0.002" tolerance, which would likely fit perfectly with my need for roughly 0.005" for the running sliding fit (no toleracnes given on the shafts).



## Gearbox Housing
I designed the gearbox housing to fully encapsulate the gears and the shafts, without having too much space. This will require an assembly in CAD with the front and back plates of the housing, the gears, and the shafts all put together. 

Here is a hand-sketch of my initial idea for the housing.


<img width="3440" height="1862" alt="unnamed" src="https://github.com/user-attachments/assets/c60ecd33-1d76-401d-9411-84873237b269" />



## Gearbox CAD Model
Starting off to create my CAD assembly, I created the input and output shaft the same way. I sketched a circle and extruded them both 1". I changed the accuracy to be 3 decimal places, since the inpiut shaft is 0.125" not 0.13". The output shaft can be seen here:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/add6f826-bc48-454b-80f8-7d4ae812c1cc" />

I then downloaded the CAD files for the two journal bearings, as well as the gears. Next was to design the actual front and back plates for the gearbox holder. I looked at the given pitch diameter values for both gears and sketched a circle of them. I coincidented the outside radiuses as seen here:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f0ef3870-944c-433d-b067-71925d84d8c2" />

I then sketched a circle from the pitch diameters of the two gears to be outwards 100 thousands of an inch for both gears to accommodate room for the outside diameters of the gears, but not have a lot of extra material.


## Lessons Learned






