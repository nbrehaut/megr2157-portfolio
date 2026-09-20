# A5 – [Bracket Design]

## Objective
Detail design a bracket to hold a horizontal force applied symmetrically by a strap outline in resource #1. The bracket’s dimensions are designed with different fit classes. Each dimension of the T beam is part of the fit:

- “a” intention for use where accuracy is not essential
- “b” is about the closest fits that can be expected to run freely
- “c” is where accurate location and minimum play is desired

Design using a safety factor of 4 and applied load in between 500 lbf < F < 800 lbf. Choose one of three metals, aluminum 6061 T6, Steel (ASTM A36), or Titanium (Ti-6Al-V4). Furthermore, state assumptions and approximations about the design in order to use fundamental strength of materials analysis. For example, use the proper stress analysis and deflection analysis where appropriate. Assume no failure due to direct shear stress. 

- Deflection is 0.005 in
- Force Between 500-800 lbf
- Safety Factor of 4
- Assume no failure due to direct shear stress.

Start with A which will drive the nominal dimensions of B and so forth
- Treat Feature A as a cantilever beam
- Treat Feature B axial loaded bar
- Treat Feature C as a simply supported beam with a concentrated load at the center
  
<img width="588" height="227" alt="image" src="https://github.com/user-attachments/assets/63ed23f4-dd45-41fb-a8dc-3d276f499c75" />


## Feature A ##
**Stress:**
Before doing any math, I decided on using [ASTM A36 Steel](https://www.azom.com/article.aspx?ArticleID=6117). To start off with the stress calculations for feature A, I referred to _Appendix A_ for formulas. I used the Z and r equations to formulate a required diameter for the shaft. This was mostly plugging in numbers. 

**Stiffness:**
For the stiffness equation, I related the formula for a uniformly loaded cantilever beam to the moment of inertia for a circular cross sectional beam. This allowed me to obtain a related equation for minimum diameter. 

**Calculations:**

<img width="1500" height="800" alt="1" src="https://github.com/user-attachments/assets/38b514ff-1d0e-4ad8-a24e-57a97fbf98d2" />

## Feature B ##
**Stress:**
For feature B, stress = F/A was used to deduce the Area into the minimum required base.

**Stiffness:**
For stiffness of feature B, I used delta = FL/EA and the given 0.005 in max deflection to find the required base size. 

**Calculations:**

<img width="1500" height="800" alt="1" src="https://github.com/user-attachments/assets/502cd122-81bd-4748-82cb-e2cc43027fb2" />

## Feature C ##
**Stress:**
Feature C's stress equations had me finding the moment of the "beam". I then plugged this moment into Mc/I. I then needed to find the moment of inertia of a rectangular beam, and plugged all of these values into my equation. To find the max allowed stress, I put the yield strength (3600 psi) over the safety factor of 4. Lastly, I set this number equal to my equation of stress relating to h and solved for h. 

**Stiffness:**
For stiffness, I used the equation for a center loaded beam and solved. For feature C, I made sure to use the highest possible values when there was a tolerance involved. This was so I could get the maximum moment value. This logic was used for everytime in this project that a tolerance was involved in a measurement.

**Calculations:**

<img width="1500" height="800" alt="1" src="https://github.com/user-attachments/assets/4e1fc3ac-950e-4810-b6c5-e977d84ab141" />

## Feature D ##
**Stress:**
Feature D's base was very straight forward to calculate in terms of the stress. I was left to choose the depth of the feature, and chose for it to be equal to the width of the bracket, making the contact area (cross section) between the bracket and the beam to be a square.

**Stiffness:**
Feature D's stiffness equation was a simple FL/EA equation, giving us our base. I also assumed the cross sectional to be a square as I did in the stress analysis.

**Calculations:**

<img width="1500" height="800" alt="1" src="https://github.com/user-attachments/assets/be0acc47-1257-460c-a556-5cf09972ed44" />

## Feature E ##
**Stress:**
Feature E also forced me to find the moment of the "beam", giving me the same moment value as Feature C. I then plugged this value into the Z equation, which then allowed me to link this value to the height of the feature.

**Stiffness:**
My stiffness equation was once again the equation for a center loaded beam. After plugging in the moment of inertia equation, I solved for the required height.

**Calculations:**

<img width="1500" height="800" alt="1" src="https://github.com/user-attachments/assets/9b6a3301-f798-4426-bc62-08679c5a8dbd" />

## Multiview Sketches

**Stress Analysis Sketch:**
<img width="1080" height="1394" alt="1" src="https://github.com/user-attachments/assets/9770c3c9-6987-43e8-8f23-2174af7ff885" />


**Stiffnes Analysis Sketch:**
<img width="1080" height="1360" alt="1" src="https://github.com/user-attachments/assets/8c4eaf77-454d-4eb6-802a-6018c53e774d" />


## Reflection
-  Governing failure mode: For at least one feature, state whether stress or stiffness governed the final dimension, and by how much (e.g., "stress required 0.25", stiffness required 0.31"). If they were close, say so — a near-tie is itself a lesson.

      _For feature A, the diameter of the shaft was heavily governed by the stress, with 1.12 inches being required compared to the 0.724 in required by the stiffness requirements._
  
-  Error propagation: Identify one instance where a value from an earlier feature carried into a later one. Did an early error (or a late catch) change a downstream result? If nothing propagated incorrectly, state what check caught it before it could.

      _The diameters that were found in the calculations for part A were carried over into their own respective analysis for part B. No early error was made as I remembered to use the correct diameter for the correct analysis._ 
  
-  Assumption sensitivity: Name one assumption you made (material choice, shear negligibility, load distribution, etc.) and describe what would change in your final dimensions if that assumption were wrong or different

      _One assumption that I made that shows up in feature D is that the width of the base of the bracket was equal to it's length (the cross sectional area is a square). My final dimensions would definitely change as this choice set the Area of the cross section to be equal to the 2.4964 inches * the features base._

## Appendix:

_**Appendix A:**_

<img width="800" height="800" alt="image" src="https://github.com/user-attachments/assets/99bc368e-ec4a-47aa-a035-43b5e5162474" />
