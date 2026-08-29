# A2 – Truss Stress Analysis

## Objective:
Design a light weight planar truss using A500 structural steel. There are four steps outlined below. Steps 1 through 2 require FBDs as well as calculations to determine the design. The third step requires a CAD model and verification of the analytical calculations in the previous steps. ( Pins not required in CAD model)

## Truss Geometry:

For the Truss's geometry, I went through a few different renditions. My first idea was a very early and brief thought of having two triangles formed by each pin, where there were truss members pointing directly vertically downwards from them, and then connecting to point D and C respectively. I decided very quickly to move on to a simpler design for the ease of this project. My next idea was very similar to what ended up being used as the final truss system, and a rough sketch is shown in this image, as well as the original idea (the original truss is on top, second idea is on the bottom). Also present in this image are some calculations for the lengths of each triangle's hypotenuse that shows up in the final truss.

<img width="800" height="800" alt="IMG_1100" src="https://github.com/user-attachments/assets/1799468a-4743-47e2-97e5-6659e1f3fd5c" />

The next step was to sketch a FBD for each pin, as well as determine the internal and external forces. This step had many redo's because of simple mistakes, and allowed for some good lessons learned. My first attempt I completed about all of the external and internal forces when I saw that the force for member BD was 0, making it a zero force member and redundant for the stability of the truss in terms of the shear force that was applied to it. The calculations can be seen in the image under this text. 


<img width="800" height="800" alt="IMG_1099" src="https://github.com/user-attachments/assets/c10ee73d-52ea-4817-9620-b8275a1b2e2b" />

My next attempt was similar but with a removal of the BD member. After completing the calculations up until the minimum cross sectional area, I went back over my work. In doing so, I realized that I had a small oversight that was very important to the numbers that I was getting. I had mistakenly assumed both of the forces were being applied downwards rather than the leftmost "P"'s arrow pointing upwards. A small mistake, but one that called for another restart of calculations. My work is shown below:

<img width="800" height="800" alt="IMG_1102" src="https://github.com/user-attachments/assets/a349bd09-f6a9-4ae9-be62-de673292d61b" />

On my 3rd attempt of the external and internal forces, I was able to calculate all of the forces up until getting to Pin C. As a part of my design process, I wanted to double check that each Fx and Fy equations would give the correct values for each member, as well as add to zero. However, I had gotten a different value for BC in pin C's FBD than the one I had calculated from pin B's. The value from pin B's FBD can be seen in the image below, and the value from pin C is not shown, however it would have been 33.3 kN of compression, a stark contrast from the previously calculated 11.1 kN of tension. After doing research on the topic and brainstorming, I determined that this could possibly be a result of removing the BD member, but decided to opt for a member connecting pins A and C the next time.

<img width="800" height="800" alt="IMG_1105" src="https://github.com/user-attachments/assets/f7ed2f14-5de6-4bb0-a199-023253b98855" />

Luckily in the fourth attempt of making the truss's FBD, I did not run into any issues. All of my calculations checked out as well as made sense. This of course included the FBD of each pin's reaction, the setup of each Fx and Fy of each pin symbolically, and the numerical solutions to each internal/external force. The lengths of the outside dimensions are present on this FBD, and the lengths of the diagonal members are located on the top right of the page rather than inside of the truss image, as to not clutter the final sketch. 

<img width="800" height="800" alt="IMG_1106" src="https://github.com/user-attachments/assets/a8f6b114-8113-4a00-b52d-56b8e0186e63" />


## Minimum Cross-Sectional Area:

Luckily, determining the minimum cross sectional area for the steel used for the steel beams went a lot smoother in terms of user errors. First I determined my knowns and unknowns which is pretty self-explanatory. Creating the symbolic formula for minimum cross sectional area was relatively straightforward. Equaling  σ=F/A and σ (allowed) = safety factor/yield since the stress we want is the allowed stress, and then solving algebraically for Amin. The next step was converting 37.97kN to pounds to get the area in square inches, I also converted it into square mm just incase I needed it later on. The Yield strength was found on google and is for A500 (assumed Grade B) steel. The calculations are shown below:

<img width="800" height="800" alt="IMG_1109" src="https://github.com/user-attachments/assets/881d38c4-e44d-45fd-a7f6-6d545f16f0ca" />

The last bit of this part of the assignment was to determine the weight of the steel in the truss. This was done by using the equation Volume = Area * Length. The total length was found by adding all of the members lengths, which were previously calculated. The area was determined in the previous step. I opted for imperial units due to the ease and familiarity. After finding the volume, I had to multiply by the density, which I found online but also cross referenced with the given example on the canvas page for this assignment. Even though it wasn't the same exact metal that was used by the previous student, it was a very familiar density which made me more comfortable with my findings. After plugging in numbers I obtained the combined weight of the steel frame without the pins.

<img width="800" height="800" alt="IMG_1108" src="https://github.com/user-attachments/assets/8d2e1ef6-821d-4021-9afc-64fb106df36d" />


## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

