# A9 – Pulleys

## Objective
The objective is to design a belt-and-pulley system that transfers power between two parallel shafts, and to size the belt, shaft, journal bearings, and frame so each has a safety factor of at least 3.

## Analyze
The task given was to design a pulley system using friction, static analysis, and stress analysis. The given information was a pulley diameter of 3 in for both pulleys, a center distance of 4 to 6 in, a speed of 1000 to 2000 rpm, a static belt tension of 4 to 6 lbf, a choice of aluminum, ABS, or steel for the pulleys, and a polyurethane belt with a yield strength of 471 psi (3.25 MPa) at 20% strain. The shaft is 1060 hardened steel.

For this assignment, my chosen values were 1500 rpm, 4 lbf, a center distance of 5 in, and aluminum pulleys. I picked 1500 rpm and 5 in because they are the middle of their ranges. I picked 4 lbf because belt stress is set by the tight-side tension, so the lowest allowed static tension gives the lowest loads on the belt, shaft, bearings, and frame. I picked aluminum because it is easy to machine, dimensionally stable, and light.

The problem does not give a friction coefficient, so I assumed μ = 0.5 for polyurethane on metal and tested other values in the Belt section.

<img width="800" height="600" alt="unnamed (2)" src="https://github.com/user-attachments/assets/125177c8-31df-4129-a370-4fa57897c6e8" />

I got started by listing out the general details of the assignment so I could organize myself.

## Belt
The first thing I looked at was the belt, because the shaft, bearing, and frame loads all depend on the belt tensions.
<img width="1008" height="1200" alt="IMG_2908" src="https://github.com/user-attachments/assets/135f391b-b9c5-4ac2-b65b-b0fa13b7a8ae" />
I started with listing my knowns and unknowns when it came to the pulleys and belt size. After that, I moved onto drawing a free body diagram to understand the system.

<img width="1008" height="1200" alt="IMG_2909" src="https://github.com/user-attachments/assets/af5f5106-f924-47da-ac7c-e8d4215d20bf" />
I finished up sizing the belt by listing out all of my equations and solving for everything unknown symbolically first. this allowed me to quickly plug in messy decimal answers to get a more accurate result. The result of the math made me choose a quarter inch diameter poly urethane belt, with a total belt length of 19.5 inches.

## Shaft
The next feature of focus was the shaft, which is 1060 hardened steel.

<img width="1008" height="1200" alt="IMG_2910" src="https://github.com/user-attachments/assets/4fd57b0f-f559-469b-bac7-f9d9c38f7057" />
I began sizing the shaft in a similar manner to the Belt. i listed knowns and unknowns and drew the problem with a free body diagram.
<img width="1008" height="1200" alt="IMG_2911" src="https://github.com/user-attachments/assets/dc37221c-04a4-46f3-83d1-026d1c8d30dd" />
After drawing the free body diagram, i solved for the minimum diameter and shear force symbolically and then plugged in my values to get my minimum diameter. I ended up choosing a 1/4 inch diameter shaft to match commonly supplied shaft sizes.

## Journal Bearing
The work flow is the exact same for the journal bearing, except I had to pit the calculated data against a chart to pick a material for my bearing. after getting my numbers, i landed on choosing porous bronze as the bearing material.
<img width="1008" height="1200" alt="IMG_2912" src="https://github.com/user-attachments/assets/6cebf1fe-ca93-434a-93d6-1aa06932c5e9" />
<img width="687" height="471" alt="Screenshot 2026-11-05 074423" src="https://github.com/user-attachments/assets/bf9691ab-cff7-4aa6-88a0-c9acbe5e0a76" />

Bearing material chart
## Frame
The last component to design was the frame that holds the pulley system.

<img width="1008" height="1200" alt="IMG_2913" src="https://github.com/user-attachments/assets/4ef17637-51bd-46b2-9ef6-a3757a18e03c" />
### Hand Calculation
The frame has to hold the two shafts exactly 5 in apart against the belt, which pulls them toward each other. I used two identical 6061-T6 aluminum bars like the Appendix A concept, one on each side of the pulleys, with a bearing pressed into each hole. Each bar is loaded in compression, and to be conservative I assumed one bar carries the full 8 lbf. The bar is 0.75 in wide and 0.25 in thick with 0.375 in holes. Net-section stress, hole bearing stress, and tear-out stress each came to about 85 psi, and Euler buckling as a pinned column gives a critical load of about 3,855 lbf. A fixed 5 in center distance cannot adjust belt tension, so I kept it fixed and let the belt length set the tension



## Communicate
the biggest engineering lesson that i learned while working on the project was how to size bearings for a pulley and shaft assembly. It took me longer than it probably should have to figure out the calculations, but I am definitly more confident after struggling through it. All in all, it took me about 4 hours to complete this assignment. this assignment was definitely one of the easier ones, as I was not required to use CAD.
