# A9 – Pulleys

## Objective
The objective is to design a belt-and-pulley system that transfers power between two parallel shafts, and to size the belt, shaft, journal bearings, and frame so each has a safety factor of at least 3.

## Analyze
The task given was to design a pulley system using friction, static analysis, and stress analysis. The given information was a pulley diameter of 3 in for both pulleys, a center distance of 4 to 6 in, a speed of 1000 to 2000 rpm, a static belt tension of 4 to 6 lbf, a choice of aluminum, ABS, or steel for the pulleys, and a polyurethane belt with a yield strength of 471 psi (3.25 MPa) at 20% strain. The shaft is 1060 hardened steel.

For this assignment, my chosen values were 1500 rpm, 4 lbf, a center distance of 5 in, and aluminum pulleys. I picked 1500 rpm and 5 in because they are the middle of their ranges. I picked 4 lbf because belt stress is set by the tight-side tension, so the lowest allowed static tension gives the lowest loads on the belt, shaft, bearings, and frame. I picked aluminum because it is easy to machine, dimensionally stable, and light.

The problem does not give a friction coefficient, so I assumed μ = 0.5 for polyurethane on metal and tested other values in the Belt section.

picture 1

I got started by listing out the general details of the assignment so I could organize myself.

## Belt
The first thing I looked at was the belt, because the shaft, bearing, and frame loads all depend on the belt tensions.
<img width="3024" height="4032" alt="IMG_2908" src="https://github.com/user-attachments/assets/135f391b-b9c5-4ac2-b65b-b0fa13b7a8ae" />
<img width="3024" height="4032" alt="IMG_2909" src="https://github.com/user-attachments/assets/af5f5106-f924-47da-ac7c-e8d4215d20bf" />


## Shaft
The next feature of focus was the shaft, which is 1060 hardened steel.

<img width="3024" height="4032" alt="IMG_2910" src="https://github.com/user-attachments/assets/4fd57b0f-f559-469b-bac7-f9d9c38f7057" />


## Journal Bearing

<img width="3024" height="4032" alt="IMG_2912" src="https://github.com/user-attachments/assets/6cebf1fe-ca93-434a-93d6-1aa06932c5e9" />

## Frame
The last component to design was the frame that holds the pulley system.

<img width="3024" height="4032" alt="IMG_2913" src="https://github.com/user-attachments/assets/4ef17637-51bd-46b2-9ef6-a3757a18e03c" />
### Hand Calculation
The frame has to hold the two shafts exactly 5 in apart against the belt, which pulls them toward each other. I used two identical 6061-T6 aluminum bars like the Appendix A concept, one on each side of the pulleys, with a bearing pressed into each hole. Each bar is loaded in compression, and to be conservative I assumed one bar carries the full 8 lbf. The bar is 0.75 in wide and 0.25 in thick with 0.375 in holes. Net-section stress, hole bearing stress, and tear-out stress each came to about 85 psi, and Euler buckling as a pinned column gives a critical load of about 3,855 lbf. A fixed 5 in center distance cannot adjust belt tension, so I [[kept it fixed and let the belt length set the tension / added a slotted hole]].



## Communicate
[[Write 3 to 5 sentences on what you took away from this assignment, in your own words and with specifics. Avoid the words "good," "bad," "easy," and "hard."]]

I compared my hand calculations to the CAD model. My calculated belt path length was 19.42 in and the path in the CAD model was [[X in]], a difference of [[Y%]]. [[Explain any difference.]]

I made the following mistake: [[describe a real mistake: what you did, how you noticed, how you fixed it, and what changed]].

Overall, this assignment took me [[X hours Y minutes]] in total, with about [[Z]] spent on [[calculations / CAD / documentation]].

Lessons learned:
- I learned that the belt has to be sized on the tight-side tension (6.62 lbf), not the static tension (4 lbf). Sizing on 4 lbf would have allowed a 3/16 in belt, which has a safety factor of 1.96.
- I learned that a round belt's tension comes from how far it is stretched, so a catalog belt 1/4 in too short would raise the static tension from about 4.4 lbf to about 5.9 lbf and drop the belt safety factor below 3.
- I learned that a bearing can be far below its pressure limit and still fail: acetal allows 1,000 psi and my load is 67 psi, yet it failed because pressure times speed (6,550) exceeded its PV rating of 3,000.
- I learned that an unspecified friction coefficient should be bounded rather than guessed once, because varying μ from 0.3 to 1.0 changed the transmitted torque but not the belt or shaft selections.
