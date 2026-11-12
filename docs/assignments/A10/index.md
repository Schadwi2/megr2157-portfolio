# A10 – Lead Screw Translating System

## Objective
This assignment was a group project where students were to work together on designing a lead screw based load tester. this is the first part of the assignment, with the second part coming in A11. A10 consists of the high level design of the tester along with the calculations to size the crosshead and lead screw for the system. We were given very broad guidelines, with our goal being accurate and repeatable load application to 2000 N with minimal deflection. our key constraints consisted of no electrical components, a 2 kN capactiy, a 1-50 mm/min speed range, to have atleast an 18 inch leadscrew, and a safety factor of 4.

## Lead Screw Diameter
-variables photo

-lead screw photo

for the material, i selected 1018 steel as that was the most common material on McMaster. I began by writing out my knowns and unknowns and figuring out what i was solving for. The goal of these calculations is the minimum diameter for the lead screw. 

### Buckling check
in order to make sure the lead screw is accurate and repeatable, i used the critical force equation for buckling to ensure the minimum diameter is enough.

-buckling photo

This revealed a larger diameter, which will be the diameter I move forward with.

## Rotation Speed

-Rotation Photo

The buckling calculations gave me a diameter of around ~10mm, which came out to .3806 in. This is an inconvenient size, so i rounded up to 1/2 inch. Looking online, a popular thread size was 1/2 - 10, which is what i went with in my calculations. this gave me my speed range.

## Torque

- torque photo

finally for the leadscrew design, i needed to account for the maximum torque it will experience. thankfully, this is given by one equation with every variable known. This equation was given by the machinery handbook.

## Screw Selection

- screw photo

## Nut and Flange
### Thread Bending

- Thread bending photo
Using the selection from McMaster as a guide, i made a choice to use 673 bronze as my material. This allowed me to calculate the thread per inch.

## Flange Selection

## Crosshead design

### Sketch

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

