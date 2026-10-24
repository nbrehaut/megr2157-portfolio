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

The only part of my data that converged this time (>7%) was the max displacement. I ran a 3rd test for this first loop with a finer mesh (35693 elements).

Here is my stress data: 
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f5cc7109-ab0e-4ff4-8c37-e407c477a10a" />

My data table for loop 1 can be seem here:



## Outer Loop 2 
For my 2nd loop I decided to make feature B thicker, as it clearly appeared to be the main cause of stress on the bracket. I thickened it 50 thousandths of an inch to 350 thousands.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/8f3c500c-5c9f-4705-9f68-82a9d51ca0cd" />


Next, I ensured that feature A was to the back of the new thickness of feature B by extruding it to the surface.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/af334df2-6875-459f-9f5d-847c0fc74713" />

I then ran my first FEA again, ensuring to also write down the new mass of the bracket. The default mesh settings called for 10176 elements.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/ae1fd414-1d19-470d-911f-2c9e8643ce2d" />

This experiment proved to be a lot better, as there was less stress and it was concentrated over multiple different areas, and not just one location. Solid works also did not call for a "high deflection" test this time, which was more evidence of an improved design. 

As seen here, the most stress on the part is in the corners connecting feature B to the physical bracket holder. This will be adressed in the next outer loop.
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/8de3e00d-86ff-4191-89c1-9ad8b40ec82b" />

The max displacement was still on feature A, which I also plan to fix in the next rendition. 
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/5081e69b-7db7-4bd0-ae85-dc5ed4091fa2" />

I also for the first time this test was returned with a safety factor above 1, meaning that my part would (in theory) not fail due to the 500lbf force. My displacement was also under 1 mm now, I saw a lot of great improvements from thickening the feature B.

For my next iteration I used a more coarse mesh that returned 2890 elements:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/340e38fa-a04a-4c02-b358-71bd55b3430b" />
Test Results for stress:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/db3e47f3-ebbe-4bde-849d-583940c75819" />

After running the test, I was given only one convergence under 7% again (roughly 23%, 3%, 17%). This led to me running another test with a mesh finer than the original. This mesh had 52278 elements. 
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/770c069f-f2e9-489b-8d90-e196afa92ed8" />

In a very interesting twist, this data proved to be under 1 for safety factor, meaning it would now likely fail. This stress FEA showed that there was a very high concentration of stress for the part at the connection of feature B and feature C (base of the top of the bracket). 

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/d28c3c8d-dce5-4a00-8be0-8d8aaf98a67f" />

These numbers also did not converge, but the 3rd test marked the end of this outer loop, as well as gave me information on what I wanted to fix for my 3rd and last outer loop.


## Outer Loop 3 

To begin the geometrical change for outer loop 3, I created a 0.25 inch radius fillet for the connections of feature B and feature A. 
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/adace367-0ac5-4d22-9f3d-e6eed720d5f3" />

I also extruded another feature B to the other side, to hopefully relieve some of the displacement done to feature A.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/09fbb529-c059-413f-b51c-ff84aa40827b" />

I made sure to filet this part's edges as well, leaving a completely symmetrical part. 

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/24bd1f40-f930-4ae5-bc8c-6503c824eaae" />



## Decide


## Communicate
A few downsides to my final design are ease of instalation for the strap itself, weight, and possibgle cost.
