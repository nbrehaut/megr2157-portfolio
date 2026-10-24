# A7 – [FEA on Bracket]

## Objective(s):
Your task is simply to create a high stiff, high strength, and lightweight component. Use Finite Element analysis to drive your decision making process throughout your design. Each step of the analysis and before you make geometric changes make sure the component’s results (stress/displacement/Safety Factor) converge on a 7% difference. Achieve this by modifying the number of elements. If after three attempts to converge use the stiffness and stress from the finer mesh size use the finest mesh size and proceed through the process.

## Outer Loop 1 
To start off my first outer loop iteration, I used the original design from assignment 5. I loaded this model into solid works, and then ran an FEA. To do this, I first started a new study. Then I applied a 500lb force onto the top of part A pointing downwards. This was done to match the bracket's original parameters from project 5 as seen here :
<img width="218" height="187" alt="image" src="https://github.com/user-attachments/assets/f83135aa-77c0-49b5-bedb-17d6133f1386" />

Getting the correct force for the model took a while, as by default solid works applied the force distributed across the rounded part of the cylinder. This included some of the 500lbf being applied upwards rather than downwards from the strap. Eventually I figured it out, as shown here :

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/ccce8537-fc9e-4bed-be94-031a4c3b3bb3" />

Next step was to generate the mesh, I used the default mesh size. There were Study 10411 mesh elements. 

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/fb71c2ac-bbd3-4d17-942a-02bf8ac46f1f" />

Then I ran the study. This process will be repeated many times, so the ongoing detail will be less for the overall process, and more about the design changes and changed solid works settings. After attempting to run the study, I realized that my material had not been applied. I quickly applied the material.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/820d4d0f-5b81-48d2-b4ca-6adc51e498cf" />

I then redid my previous steps, fixed the top of the inside of the bracket and ran the study.

Fix:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/1a22de4f-a519-4b62-af51-b6c647cce6c7" />

My results are shown here:
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/c316bc39-2bfd-44d1-9cc6-437b8b8132d1" />

My feature B was clearly the bottleneck in this test. I then ran a test again with a more coarse mesh. There were 2794 elements in this mesh. Here is my displacement data this time:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/48b38ae6-8fb5-4193-b5ff-fbb85003e4f4" />






## Outer Loop 2 

## Outer Loop 3 


## Decide


## Communicate

