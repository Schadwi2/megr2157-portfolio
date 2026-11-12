# A10 – Lead Screw Translating System

## Objective
This assignment was a group project where students were to work together on designing a lead screw based load tester. this is the first part of the assignment, with the second part coming in A11. A10 consists of the high level design of the tester along with the calculations to size the crosshead and lead screw for the system. We were given very broad guidelines, with our goal being accurate and repeatable load application to 2000 N with minimal deflection. our key constraints consisted of no electrical components, a 2 kN capactiy, a 1-50 mm/min speed range, to have atleast an 18 inch leadscrew, and a safety factor of 4.

## Lead Screw
### Lead Screw Diameter

<img width="459" height="597" alt="Screenshot 2026-11-12 055646" src="https://github.com/user-attachments/assets/1878ee90-0e0a-4296-a9b9-e7b42f0345d7" />

for the material, i selected 1018 steel as that was the most common material on McMaster. I began by writing out my knowns and unknowns and figuring out what i was solving for. The goal of these calculations is the minimum diameter for the lead screw. 

#### Buckling check
in order to make sure the lead screw is accurate and repeatable, i used the critical force equation for buckling to ensure the minimum diameter is enough.

<img width="454" height="609" alt="Screenshot 2026-11-12 055652" src="https://github.com/user-attachments/assets/7a16c89d-e6dc-48f2-95eb-e2e1424ae838" />

This revealed a larger diameter, which will be the diameter I move forward with.

### Rotation Speed

<img width="458" height="602" alt="Screenshot 2026-11-12 055657" src="https://github.com/user-attachments/assets/af5342fd-f77b-4387-9852-25653ff12f5a" />

The buckling calculations gave me a diameter of around ~10mm, which came out to .3806 in. This is an inconvenient size, so i rounded up to 1/2 inch. Looking online, a popular thread size was 1/2 - 10, which is what i went with in my calculations. this gave me my speed range.

### Torque

<img width="457" height="525" alt="Screenshot 2026-11-12 055702" src="https://github.com/user-attachments/assets/e6d426d2-6034-4103-879d-1a1805d53eaf" />

finally for the leadscrew design, i needed to account for the maximum torque it will experience. thankfully, this is given by one equation with every variable known. This equation was given by the machinery handbook.

## Screw Selection

<img width="451" height="476" alt="Screenshot 2026-11-12 055710" src="https://github.com/user-attachments/assets/196d4c9c-0866-4c0a-bd40-1397370de9f3" />

## Nut and Flange
### Thread Bending

<img width="451" height="476" alt="Screenshot 2026-11-12 055710" src="https://github.com/user-attachments/assets/196d4c9c-0866-4c0a-bd40-1397370de9f3" />
Using the selection from McMaster as a guide, i made a choice to use 673 bronze as my material. This allowed me to calculate the thread per inch.

## Flange Selection

## Crosshead design

<img width="455" height="560" alt="Screenshot 2026-11-12 055715" src="https://github.com/user-attachments/assets/08857639-5685-43be-8d9f-7b98e50a23de" />
### Sketch
<img width="461" height="547" alt="Screenshot 2026-11-12 055720" src="https://github.com/user-attachments/assets/12d905e0-0083-4bb1-9920-568a0f2f2a2e" />
## Costs

## CAD

### Crosshead
-crosshead
-equations
### Leadscrew

### Nut / Flange

### Frame

### Assembly

## 2157

## Crosshead Drawing

## FEA 

## Decide
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## Communicate

