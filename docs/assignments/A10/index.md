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

## Nut and Flange Selection
<img width="782" height="550" alt="Screenshot 2026-11-12 060200" src="https://github.com/user-attachments/assets/a5de40d6-078d-4aaf-8ec9-c0ad935ca637" />
<img width="765" height="545" alt="Screenshot 2026-11-12 060153" src="https://github.com/user-attachments/assets/2743d2be-6291-46fd-baff-8d89ae158782" />
I found these parts online and made sure they fit the properties outlined by the calculations i made. I have noted the dimensions and the CAD files will be used later in the project.
## Crosshead design

<img width="455" height="560" alt="Screenshot 2026-11-12 055715" src="https://github.com/user-attachments/assets/08857639-5685-43be-8d9f-7b98e50a23de" />
In order to properly design the cross head, i needed to find the height. to find the height, i needed to consider both the stress it would experience and the deflection of the crosshead itself. I did calculations for both and it came out that deflection was the limiting factor.

### Sketch
<img width="461" height="547" alt="Screenshot 2026-11-12 055720" src="https://github.com/user-attachments/assets/12d905e0-0083-4bb1-9920-568a0f2f2a2e" />

This is a sketch of the crosshead i designed. it features a top, right, and front view.
## Costs
 <img width="990" height="300" alt="Screenshot 2026-11-12 060542" src="https://github.com/user-attachments/assets/166aa3b3-e04d-440e-8980-472656eea408" />
This is the total costs for my design, with links attached to where they can be sourced.
 link to file for excel

## CAD

### Crosshead
<img width="1707" height="1035" alt="Screenshot 2026-11-12 050843" src="https://github.com/user-attachments/assets/45e22b85-d4d9-4f6f-bfb3-8bd82db9cef1" />
<img width="1472" height="385" alt="Screenshot 2026-11-12 050854" src="https://github.com/user-attachments/assets/1356dea5-78f1-43a3-bad1-5df9f0219696" />
### Leadscrew
<img width="1868" height="996" alt="Screenshot 2026-11-12 061204" src="https://github.com/user-attachments/assets/cb00c4ae-525d-4fe0-b823-1d1fdd6d585c" />

### Nut / Flange
<img width="1418" height="967" alt="Screenshot 2026-11-12 051405" src="https://github.com/user-attachments/assets/f9122292-2b4b-4cea-98e3-5b28c2c79d7b" />

### Frame
<img width="990" height="1102" alt="Screenshot 2026-11-12 050628" src="https://github.com/user-attachments/assets/f369fe9a-e86c-44bd-81fe-b933c74d2027" />

### Assembly
<img width="2311" height="1216" alt="Screenshot 2026-11-12 050153" src="https://github.com/user-attachments/assets/cdd4fe0c-2f22-4c37-ad89-4021326d6c99" />

## 2157

### Crosshead Drawing
<img width="1410" height="1091" alt="Screenshot 2026-11-12 062121" src="https://github.com/user-attachments/assets/744f129c-6cc2-46a6-87f7-c9d487929cf2" />
### FEA 

## Lessons learned
This assignment was a very long one, and it was personally very difficult for 2 reasons. The first was the fact that I did not have a team for it, when it is intended to be a team assignment. I missed the day teams were assigned and by the time I was concious of the assignment, there was no way of finding a team, so I just did the assignment solo. The second thing that made it very difficult was the CAD heavy portion of the assignment. I struggle severely with CAD software and doing anything precise, so every move in SolidWorks was a wrestle and just added time onto the assignment. Id say total time spent on the assignment is north of 14-15 hours.
## Links
CAD files : 
Cost Spreadsheet with links : 
Drawing : 
