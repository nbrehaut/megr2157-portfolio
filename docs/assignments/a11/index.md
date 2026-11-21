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



## Motor Selection and Attachments - Bryson Bare

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



## Design Floating Bearing Mount

## Bill of Materials and Labor costs 


## Lessons Learned
