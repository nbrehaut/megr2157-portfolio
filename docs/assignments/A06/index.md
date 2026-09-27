# A6 – [Bracket Drawing]

## Objective
- Create a parametric model of your bracket from A5, as well as an engineering drawing.
- Generate a comprehensive solid model and a multi-view engineering drawing that accurately represents your designed bracket.
- Incorporate all features to ensure both strength and stiffness requirements are met.

## Parametric Design
To start off my solid works model of the bracket from A5, I first chose to design based off of my calculated values for stress rather than stiffness. I then input all of my values for the parametric equations:

<img width="1920" height="1200" alt="Screenshot (71)" src="https://github.com/user-attachments/assets/2bce8398-1964-4808-9660-e92adde0a53c" />

My next step was to physically model the bracket. I started off by creating a cube that was the same dimension of my hand drawings from A5. 

<img width="1920" height="1200" alt="Screenshot (72)" src="https://github.com/user-attachments/assets/924067b9-d1d3-4a65-b1db-8ac2ee85411c" />

Next, I created the cutout for the bracket using my sizes calculated from A5 for feature B and C, as well as the width of the rigid T beam. 

<img width="1920" height="1200" alt="Screenshot (73)" src="https://github.com/user-attachments/assets/f37fca09-099c-49d8-8d88-89a12acf2f71" />

<img width="1920" height="1200" alt="Screenshot (74)" src="https://github.com/user-attachments/assets/78cfc06b-a985-4a1d-8137-582d162c8045" />

My next step was to extrude from the base of the model. This would become feature B. 

<img width="1920" height="1200" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/4fe01209-49d8-4ed4-9c6d-6b9f505ccb5e" />

I calculated the height of the extrude by using the chosen value of 1.25 inches from assignment 5, and added the radius of part A to the height. This can be seen in this photo:

<img width="1920" height="1200" alt="Screenshot (76)" src="https://github.com/user-attachments/assets/0a0b7d59-a02f-4504-b618-320a89ff5c64" />

After this, I created feature A as an extruded cylinder.

<img width="1920" height="1200" alt="Screenshot (77)" src="https://github.com/user-attachments/assets/3e7329be-5858-49a5-9329-3cd6cca23c32" />

I extruded this cylinder up to the surface of the front of the bracket mount.

<img width="1920" height="1200" alt="Screenshot (78)" src="https://github.com/user-attachments/assets/ffda90c5-c0aa-41be-8df1-e1447f798a9e" />

I then realized that feature A stuck out the thickness of feature B from the base of feature B.

<img width="1920" height="1200" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/f5020bcf-724c-4b79-960e-b37bf1517e26" />

To account for this, I extruded backwards 0.05 inches.

<img width="1920" height="1200" alt="Screenshot (79)" src="https://github.com/user-attachments/assets/8a89e8b2-9a12-44ce-aa74-d0bef50956ef" />

This left me with my finished model

<img width="1920" height="1200" alt="Screenshot (81)" src="https://github.com/user-attachments/assets/6fd3b14c-3123-4635-afad-899f11c40927" />


## Drawing

 Most of the design process for the drawing portion of this assignment was reactively straightforward. I used the ANSI template A for my design and installed the given tolerance from the canvas assignment page. I used the tolerance for the hole's base due to the bracket that I calculated from A5. I also ensured that the values that had 3 decimal places were changed to 3 decimal places rather than the program's default 2 decimal places. Here is an image of the final drawing:

<img width="473" height="365" alt="Screenshot 2026-09-27 190405" src="https://github.com/user-attachments/assets/2ba13633-04cd-41aa-9dab-de06f5c5a2d2" />



## Reflections

- One main engineering lesson that I learned is the importance of tolerances. In this project, miscalculating the tolerances could lead to the brackets' users to get injured.
- One tolerance that I hand calculated was the tolerance for the width of feature C. This dimension controlled the width of the cut that holds the rigid t beam in place. I calculated this tolerance by adding together one of dimension A's tolerance and two of dimension B's tolerances.
- One place where I applied a tighter tolerance was feature C's thickness. This was because in the hand calculations, the result was to 3 decimal places. This was a result of adding together values of 3 decimal places. One dimension that I applied a looser tolerance was the diameter of feature A. This was chosen to do because the tolerance of the part was not that integral to the design, so I decided to save a little bit of cost on somewhere that may not be hindered that much.

This project took me roughly 2 hours to complete from start to finish.

[Google Folder with CAD Files](https://drive.google.com/drive/folders/1XZeDiHqGNRlu-JgQssnBpCSPFCLwoiCg?usp=sharing)
