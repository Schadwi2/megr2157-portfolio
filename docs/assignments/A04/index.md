# A4 – Motor Mount

## Objective
To design a motor mount that could hold a specified motor when attached to a wall via 4 mounting screws.

## Analyze
The given information includes a specified safety factor of 3, a force of 300N, a max deflection of .3 mm. I chose my material to be ABS, which comes with a young’s modulus of 2000 MPa and a  yield strength of MPa. I was given a drawing of the motor, so i will be using that as a preliminary resource to size the motor mount. This tells me what each of the features length and width will be. 

<img width="816" height="426" alt="Screenshot 2026-09-17 021005" src="https://github.com/user-attachments/assets/0c859065-5be5-4b75-9aea-5fd0d87e5a2a" />

### Feature 1
I started feature one by realizing i needed to find the dimensions of the plate first and foremost. To begin, i laid out some useful equations that i will use to find the thickness of the plate. My starting point was the drawings of the motor from Appendix A, which gave me the amount that the shaft protruded, as well as how far apart each of the screws were, 22mm. I added 5 mm to the radius, making my b = 32mm. I calculated the moment by using the length of protrusion times the force, giving me 5400 N-mm. My unknowns now are the max stress and h. I found max stress using my material properties and the supplied safety factor, giving me 10MPa. As shown Below, I solved for h two different ways, one based off the max deflection and the other based off the max stress. The largest of the two was 12 mm. 

<img width="1008" height="1344" alt="IMG_2711" src="https://github.com/user-attachments/assets/506a5885-e314-4895-b824-b2935036a7dc" />

### Feature 2
Feature 2 uses the same equations to find its thickness, but two of the values change. These are L_2 and M.  For M, i used the same 18mm, but added L2 to it for the calculation. For L_2, I added the thickness i found in the last step to L_1, giving me 44 mm. Using that for the moment, i got 18600 N-mm. Utilizing the same thickness equations, I arrived at 20.152 mm being the minimum thickness. 

<img width="1008" height="1344" alt="IMG_2712" src="https://github.com/user-attachments/assets/9e093768-6c3d-48a7-ad61-253aecfc4257" />


## Visualization

<img width="1008" height="1344" alt="IMG_2713" src="https://github.com/user-attachments/assets/4ffc9736-e030-485c-9191-482afa695b22" />

### CAD

I started off by ensuring all of my equations and different variables were inserted into my software. 

<img width="809" height="525" alt="Screenshot 2026-09-17 064751" src="https://github.com/user-attachments/assets/e7c2e9fc-320c-4183-bc6d-c6e67f78c74b" />

I then started it off by making the block that will become feature 1

<img width="1286" height="975" alt="Screenshot 2026-09-17 053909" src="https://github.com/user-attachments/assets/ec24490c-4c75-4d01-aca6-0b7dc765ecdf" />

After that, I proceeded to make the indent for the motor to rest on.

<img width="1239" height="1117" alt="Screenshot 2026-09-17 053919" src="https://github.com/user-attachments/assets/52478d09-ae10-4eac-a8a7-f9042675c5de" />
then I put in the 5 different holes that feature one requires, 4 screw holes and one in the center for the shaft of the motor.

<img width="1299" height="1269" alt="Screenshot 2026-09-17 055052" src="https://github.com/user-attachments/assets/ecef9a5a-5ed3-4445-bf77-23527ec34237" />

That marks feature 1 done, so i started feature 2 by adding a box to the side of feature 1

<img width="1323" height="1161" alt="Screenshot 2026-09-17 055650" src="https://github.com/user-attachments/assets/6b2cecb2-6b72-4a08-8203-0804d0d17d8a" />

finally, I finished off the model by adding the four mounting screws to feature 2. It was at this point that I added a variable for the width of the screws on feature 2, and I named it "width".

<img width="926" height="1062" alt="Screenshot 2026-09-17 060259" src="https://github.com/user-attachments/assets/1192fb97-2c78-4cd9-850f-de4c647fce1a" />

## 2157
### Multiview Drawing
<img width="1006" height="781" alt="Screenshot 2026-09-17 065339" src="https://github.com/user-attachments/assets/8fc2ae0f-1ef5-493f-a554-ba60fdf9dc5d" />

## Lessons Learned
I had a lot of trouble with using SolidWorks still as I really only have experience with Creo and Revit. The biggest hang-up was trying to figure out how to make a drawing. The assignment all in all took me around 4 hours.

### CAD Download






