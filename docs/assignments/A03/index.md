# A3 – [Parametric and FEA]

## Objective
Use axial deflection modeling to design its dimensions

Use parametric design to determine a bars length

Introduce you to FEA (Finite Element Analysis)

Introduce you to linking dimensions to appropriate parameters in CAD.

Compare and contrast the different analysis

You are to design a bar which has a circular cross section where the values of the criteria given for the material, maximum deflection, and load. Determine the bar’s minimum geometry (ie.. length, diameter, and weight) through parametric design while under direct tension. Then verify the geometry through finite element analysis.

Our bar's material must be an aluminum with a modulus of elasticity between (8.5 and 11.5)*10^6 (mega) psi. The max axial deflection is 9 thousandths of an inch (0.009 inches).

## Hand Calcultions:
My first step in this project was to choose a diameter for the beam that would satisfy all of the requirements of stability for the beam. I decided to use a half of an inch for the ease of calculations. Next, I searched through solid works and found an aluminum that fit the requirements of young's modulus. This material was 1060-H18. Lastly I used 500lbf in all of my calculations to ensure the beam could withstand any forces within the project's parameters. Next was to preform hand calculations. I calculated the cross sectional area, and used this value to help me solve for the required length of the beam. The latter was done using the direct tension elongation equation. These hand calculations can be shown below:

<img width="800" height="650" alt="unnamed" src="https://github.com/user-attachments/assets/48bd550e-9050-4399-a203-775f9eff6353" />


## Parametric Desigm:
After my hand calculations I moved on to the solid works modelling. My first step in this process was creating a circle sketch in the front datum plane that had a diameter of 0.5in. 

<img width="1920" height="1200" alt="2" src="https://github.com/user-attachments/assets/757da96c-4a2e-4a0d-aaad-ff925149ae16" />

The next step was to extrude this circle by 35.37 inches long. 

<img width="1080" height="675" alt="2" src="https://github.com/user-attachments/assets/cd3ccd48-30a2-4744-8e06-fed6c938f006" />

Next, I assigned the material of 1060-H18 to the beam.

<img width="1080" height="675" alt="2" src="https://github.com/user-attachments/assets/efbd89a7-44a8-4123-9966-1f8083c8305d" />

Lastly, I created all of the variables inside of solid works and ensured that my math checked out with my previous hand calculations.

<img width="1920" height="1200" alt="2" src="https://github.com/user-attachments/assets/09a62ce8-26d8-4516-9b70-d75a248b574e" />

## Finite Element Analysis (FEA):
To start the FEA in solid works, I first had to start a new study. After this, I then had to apply a fixture force to one end of the beam as shown here:

<img width="1080" height="675" alt="1" src="https://github.com/user-attachments/assets/4fac99fa-9bd2-47b7-8bf1-fe37379c80e4" />

Next, I applied a 500lbf pulling force to the other end. At first, the force was pushing into the beam, but I selected "reverse direction" to ensure the force was pulling. 

<img width="1080" height="675" alt="1" src="https://github.com/user-attachments/assets/d287d0ad-fdf3-411c-8a43-3d59dfdba1ff" />

Following this, I conducted the study. This gave me access to 3 different maps. The first of which being the deflection map: 

<img width="1080" height="675" alt="1" src="https://github.com/user-attachments/assets/dbf41f07-d7ac-4995-8584-4af899b3d217" />

The last one used in this assignment was the von Mises stress map:

<img width="1080" height="675" alt="1" src="https://github.com/user-attachments/assets/18ca0508-fc46-4291-ada4-f3a8779b4ae7" />

The maximum stress was 2693 psi from the von Mises, and yield strength of the beam was calculated to be 18130 psi. The safety factor is calculated by dividing the yield strength by the von Mises strength, giving us a safety factor of 6.73.

## Reflection:

The axial deflection of the beam that I calculated was 0.009 in, as I used the maximum deflection for my calculations. Solid works gave a 0.009004. The percent difference is a 0.04% difference, likely due to rounding. This means the beam acted exactly as I had calculated. I believe that these numbers are so similar due to the very basic calculations that were done behind the scenes. Since solid works and I both assumed that the left side of the beam is fixed, and there is a perfectly uniform 500lbf force being applied on the opposite end, there is not much room for the numbers to get mixed up, except for rounding of my calculator or the CAD program. Personally, for this specific application, I would trust solid works more than hand calculations. The only reason for that is because it gives more information than the hand calculations that I did. If there was a 
