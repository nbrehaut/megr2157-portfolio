# A2 – Truss Stress Analysis

## Objective:
Design a light weight planar truss using A500 structural steel. There are four steps outlined below. Steps 1 through 2 require FBDs as well as calculations to determine the design. The third step requires a CAD model and verification of the analytical calculations in the previous steps.

## Truss Geometry:

For the Truss's geometry, I went through a few different renditions. My first idea was a very early and brief thought of having two triangles formed by each pin, where there were truss members pointing directly vertically downwards from them, and then connecting to point D and C respectively. I decided very quickly to move on to a simpler design for the ease of this project. My next idea was very similar to what ended up being used as the final truss system, and a rough sketch is shown in this image, as well as the original idea (the original truss is on top, second idea is on the bottom).The reason I ended up choosing this design for the final truss was the simplicity and effectiveness. Also present in this image are some calculations for the lengths of each triangle's hypotenuse that shows up in the final truss.

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

## Cross-Sectional Area of Pins:

In the first step of part 3, I had to list the knowns and unknowns. Next, I had to draw a quick FBD of a pin under single shear stress. Next I had to solve symbolically for the cross sectional area of the pins, which I did by relating the shear stress equation with the definition of a safety factor, as done before. Next I plugged in all of the values that I was either given or determined previously to get the minimum cross sectional area of each pin. Lastly, I solved for the diameter of each pin for use in CAD, then plugged values into W=pV for the weight of the pins. This was initially in terms of length since I had not yet determined the length of the pins, but originally planned to have pins be around 2.75 inches, which would have the weight be roughly 0.3 pounds. All of my calculations (as well as the FBD of a pin) can be seen below:

<img width="800" height="800" alt="IMG_1115" src="https://github.com/user-attachments/assets/a5e5335e-1a3b-4840-ba10-511a0bc92c27" />


## CAD Model of Truss System: 

To start my CAD model of the metal frame of the truss system, I first made a simple extrude of a rectangle along the front plane. I also made an extrude under this one later, these two extrudes acted as my AB and CD members. Member AB can be seen below:

<img width="1920" height="1200" alt="Screenshot (30)" src="https://github.com/user-attachments/assets/62d07517-e6fa-448f-ade7-012eb4bd0bad" />


Next, I brainstormed many different ways to create a pin connection at the intersection of the members. Here are some early design ideas that I had such as modeling a pin joint (scrapped due to complexity) and a circular endcap for the members (scrapped due to the pins becoming ineffective). You can see an early idea of my final design choice, as well as unfinished math that would have determined the angle between the members (rendered useless).

<img width="800" height="800" alt="IMG_1123" src="https://github.com/user-attachments/assets/c3f6d645-7b8b-44ed-8723-d2e51d7b92c8" />

 As you can see here, I ended up modeling the circular joint before realizing that it voided the parameters of this project (using pins instead of essentially welding the members together)

 <img width="1920" height="1200" alt="Screenshot (32)" src="https://github.com/user-attachments/assets/5c22e37f-5d37-459e-9da6-5029d40f63e4" />


After scraping this idea, I decided to just move ahead and create the members, instead of figuring out their connections before. This ended up sparking an idea for me, and that was to simply physically connect them inside the Creo model, and slide the pin between the two. As I was modeling the AD member, I was brainstorming on how to physically model the connection, and originally I had the idea to use an arc as seen here:

<img width="1920" height="1200" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/5b480108-0f1b-4008-a4a4-63dc6c7b37da" />

Seen on this image is a calculation for the pin's combined weight (since I had changed the length I needed due to the pin connection design) and some conversions I needed for the pin's diameter to match the minimum cross sectional area determined earlier in the project.

<img width="800" height="800" alt="IMG_1124" src="https://github.com/user-attachments/assets/d543c1a2-fb84-4673-a51a-2dcc791fae29" />

After completing the last connection, my next idea was to make a plane in the center of the CD member, and using it to mirror the previously made AD member across into member BC's correction position. This allowed me to speed up the process, and the plane can be seen here highlighted in green:

<img width="1920" height="1200" alt="Screenshot (34)" src="https://github.com/user-attachments/assets/479af14e-9d19-4f67-89f4-a1d2d0a901f1" />

The next challenge was centering the AC component beam, and after a lot of trial and error of constraints, I ended up putting a centerline from pin A to pin C and constraining distances from it to create a centered AC member. These constraints aas well as the centerline can be seen here:

<img width="1920" height="1200" alt="Screenshot (37)" src="https://github.com/user-attachments/assets/86ce7d1b-e1c5-4530-8163-216d57fc7edf" />

While doing this, I also figured out that a better solution to the precious problem of physical connections between the members within the model was to create lines (making sure that the thickness of the beams stayed at the calculated 21mm). 

<img width="1920" height="1200" alt="Screenshot (38)" src="https://github.com/user-attachments/assets/06bfec5b-2c45-462b-a851-a2d559cd2b5b" />

After finishing the truss's model, I realized that I had modeled the member AB from the top view rather than the front, meaning I had to extrude out holes for the pins rather than simply cutting them out of the sketch.

<img width="1920" height="1200" alt="Screenshot (39)" src="https://github.com/user-attachments/assets/510cc44a-37ad-4d6e-a1b8-3fc73ed417ea" />

After a lot of tricky constraints, the holes were all cut out of the steel and the steel frame of the truss was finished.

<img width="1920" height="1200" alt="Screenshot (43)" src="https://github.com/user-attachments/assets/4230c6cd-6b41-4dbf-a366-87e586ef6f8c" />
<img width="1920" height="1200" alt="Screenshot (41)" src="https://github.com/user-attachments/assets/8ab0b0af-ddfd-46a6-a7b0-4946a8415153" />
<img width="1920" height="1200" alt="Screenshot (40)" src="https://github.com/user-attachments/assets/3864ef0f-2ce7-45a7-a456-8bab828ee8b4" />

The pin was a very simple extrude downwards from the top plane

<img width="1920" height="1200" alt="Screenshot (45)" src="https://github.com/user-attachments/assets/696bde2c-5368-41fb-9d21-7ec6263cebc4" />

Now it was time for the final assembly to be put together. In doing so, I had to constrain the front of the steel frame to the front plane of the assembly. Next, I added all of the pins into their respective spots, constraining the sidewalls of the pin into the sidewalls of the holes cut into the steel. I also constrained the front surface of the pin to the front surface of the frame. Both constraints can be seen here:

<img width="1920" height="1200" alt="Screenshot (46)" src="https://github.com/user-attachments/assets/cff8d0cf-33a8-409f-9e68-1ecc9846f81e" />
<img width="1920" height="1200" alt="Screenshot (47)" src="https://github.com/user-attachments/assets/f9d5f36e-f95b-4d55-ac07-1345fdf601a7" />

After running into a few hiccups whilst creating the materials of the AS500 Grade B and hardened tool steel, I finally was left to only let Creo calculate the weight of the truss and compare it to my own. However, I was given a very large number. After around a half an hour of troubleshooting, I had to mess with the settings of units very many times to convert back into mm instead of inches, as to not mess up my measurements. I also had to remodel the pin with the correct units, since that prt file would not cooperate (Thankfully it was the pin and not the steel frame). Here is my rendition of the necesssary values for A500 Grade B steel:

<img width="1920" height="1200" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/f9b9d35d-9282-4b80-9583-5189c41c67b7" />

Lastly, I let Creo calculate my mass and this can be seen here:

<img width="1920" height="1200" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/afd442ed-f418-402e-9603-f0395831ee1c" />

After some very basic math, I learned that my percentage error of hand calculated weight and the weight calculated by Creo was only a 1.48% error (which could be due to rounding). 

<img width="800" height="800" alt="IMG_1125" src="https://github.com/user-attachments/assets/d219c818-b5d8-46bc-84d1-2f3372127155" />

Here is an image of the final truss put together, as well as the files to download each prt file and the asm file:

<img width="1920" height="1200" alt="Screenshot (48)" src="https://github.com/user-attachments/assets/bda431a8-3faa-47d0-a760-30b56e3463fd" />

download







## Engineering Lessons Learned:


## Communicate

