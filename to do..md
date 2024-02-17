no need to them at order, ofc that depends on each item in the list.

dont push yourself too hard.

1. cut all the engine audio clips to 1 seconds or less. which if all the cars are factored in, each with separate and unique engine audio, it will add to less than 40mbs. [[engine audio files]]
2. make a garage, a really simple one. [[main garage]] 
3. Add a test car and test all the new physics stuff on it like 6dof joints. [[test car for physics]]
4. remove all the old maps. for multiple reasons.
5. make the awareness raycast rotate around to the car to emulate multiple raycasts without the increased performance requirements.
6. make the camera rigidbody and use 6dof joint to attach it to the car.
7. move the physics code to C#, but only the physics code and nothing else.
8. A dot next to the car that flashes red based on whether or not the player is going too fast before a certain corner.
9. add a lap system to the event manager and event data.
10. different camera option, only add a bumper camera.
11. control mapping option.
12. save data for the options.
13. smoke particles.
14. skid marks.
15. brake and headlights.
16. Complete the car variable editor, the weight, forward friction and assists tab.
17. use 6dof joint for the 3D ui to make it more dynamic.
18. remake all the cars to be alot, and I mean alot more higher quality, even with half modeled blacked out interiors. start with the wasp. 
	1. name all the game objects accordingly
	2. make an ambient occlusion texture.
	3. make seperate materials for headlights and backlights
	4. make blacked out blocky interiors.
	5. make bespoke wheels with brakes and very basic suspension.
	6. make side mirrors.
	7. actually model the innards of the cars like the radiators and engine headers.
	
	keep the esr (ford gt 2006) and build upon it. because its the only car that looks professionally made.
19. add new cars like the:
	1. seat leon -> spanish revolver.
	2. lotus elise series 1 -> demonica act 1.
	3. mini cooper -> small car
	   
	   this cars are the only ones you can quickly get it over with while modeling, since they're just starter cars that would probably never be used after the first boss is defeated.
	4. ferrari enzo -> red stallion
	   
	   this car is only car where you take as much time modeling as you can. because this is probably gonna be the pseudo cover car.
	   
1. make new maps, check [[what maps to make]]
2. energy recovery system (ers):
	this acts in the same way as burst nitrous, but the power of the burst is in how much energy is in the system, you gain energy by braking, the higher your speed while breaking, the more speed you lose, the bigger the energy, and the bigger the burst.
	
	it also works in a way that energy gain is exponential, the difference between 150 and 160 is much much more than 90 and 100, even tho they're both 10 apart.
22. make the boss cars. check [[boss plan]]