# A3 – Parametric and FEA

## Objective
The objective is to parametrically model a tube and perform FEA on it.


## Analyze
The task given was to design a hollow beam with a circular cross section. The given information consisted of the material, maximum deflection, and load. we were tasked with determining the length, diameter, and thickness. 

### Hand Calculation
The first step I took was to model the problem by hand and write out my known variables, my unknown variables, and my governing equations. I chose for my load to be 400 Lbf, and my material was aluminum 6061-t4, which had a Young's Modulus value of 10007604 Psi. In order to keep things simple calculation-wise, I chose for the outer diameter, d_1, to be 1 inch. I chose my thickness, t, to be .2 inches. After finding what variables were known and unknown, I had to determine what my governing equation would be. The governing equation is the axial deformation formula which is pictured. The ultimate goal of this equation was to help me calculate the maximum length of the beam to stay under the maximum axial deformation.

<img width="2380" height="3264" alt="unnamed (1)" src="https://github.com/user-attachments/assets/a1bda90c-d09c-4fb7-bb22-d9f049add04d" />


### CAD
The next step was to parametrically model the tube in solidworks. I achieved this by first setting up my global variables that follow the same flow as my hand calculations.

<img width="802" height="378" alt="Screenshot 2026-09-10 070823" src="https://github.com/user-attachments/assets/350740e7-5b2b-4a62-ac34-0f8b85b4d5f6" />


After that, I went ahead and modeled the tube in 3d using the variables I had defined.
<img width="2216" height="1129" alt="Screenshot 2026-09-10 060446" src="https://github.com/user-attachments/assets/aa41ca59-b20f-46f2-933a-bcc12e1863fa" />

## FEA
The next step in the problem was to conduct an FEA and generate a deflection map and a von Mises Stress map. The process for creating both was the same, I input where forces would be holding the beam, such as the fixed end and the force applied to the end, and created a mesh. After that, solidworks generated both of maps simultaneously.

### Deflection Map
The most notable part of the Deflection map is that it says the maximum deflection is .01 inches, which is larger than the .009 listed in the requirements.
<img width="1338" height="518" alt="Screenshot 2026-09-10 071532" src="https://github.com/user-attachments/assets/1773f634-9005-4ded-b470-ca2c8e0e2edc" />


### Von Mises Stress Map
The most notable part of the Stress map is that it tells us the maximum stress at any given point, and in this case that number was 973.2 psi. The yield strength is 40,000 psi, which ends up yielding a safety factor of 41.1.
<img width="1383" height="572" alt="Screenshot 2026-09-10 070913" src="https://github.com/user-attachments/assets/aaad08b5-0374-447c-ad40-ea55ce680a17" />

## Reflection
The axial deflection used in my hand calcs was .009 inches, but the FEA yielded a deflection of .01, which is a 11.1% difference. One reason I can find for this discrepancy is an inadequate mesh size. I would trust the hand calcs more as they work best for simple geometries such as this tube.

## Lesson Learned
I took around 5 hours to complete the assignment. the greatest lessons were learned in solid works, as i have never used the software before the semester. Learning how to use the global variables is the most important lesson learned. One mistake that took a while to correct was ensuring I used the correct formulas in the equation editor.

## Modify Design Parameters

The last thing left to do is to repeat the FEA but with a different Load and different cross sectional area. I am using the same variables/equations, but i am changing the thickness to .05, the diameter to .75, and the load to 450. My prediction was that the length would decrease. The safety factor significantly decreases after these changes, dropping from a 41.1 to an 9.0. The length also significantly dropped from 113 inches to 22 inches.

### Deflection Map
<img width="1317" height="488" alt="Screenshot 2026-09-10 070523" src="https://github.com/user-attachments/assets/a79682cd-2d90-4fc9-86fc-665da52df636" />


### Von Mises Stress Map

<img width="1289" height="455" alt="Screenshot 2026-09-10 070434" src="https://github.com/user-attachments/assets/e111ece2-0e81-4d52-912b-457bd54693d8" />

## CAD File Link
[Download CAD file](assets/files/A3.SLDPRT)



