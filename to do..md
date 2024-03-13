no need to them at order, ofc that depends on each item in the list.

dont push yourself too hard.

1. cut all the engine audio clips to 1 seconds or less. which if all the cars are factored in, each with separate and unique engine audio, it will add to less than 40mbs. (VFX)
2. Add a test car and test all the new physics stuff on it like 6dof joints. [[test car for physics]] (P)
3. remove all the old maps. for multiple reasons. (world)
4. make the awareness raycast rotate around to the car to emulate multiple raycasts without the increased performance requirements. (AI)
5. make the camera rigidbody and use 6dof joint to attach it to the car. (VFX)
	- by the camera I mean add a misc rigid body to the car itself with a 6dof, to every car. and just make the camera copy its transform.
6. move the physics code to C#, but only the physics code and nothing else. (P)
7. add a lap system to the event manager and event data. (misc)
8. different camera option, only add a bumper camera. (VFX)
9. control mapping option. (misc)
10. save data for the options. (misc)
11. smoke particles. (VFX)
12. skid marks. (VFX)
13. brake and headlights. (VFX)
14. Complete the car variable editor, the weight, forward friction and assists tab. (misc)
15. remake all the cars to be alot, and I mean alot more higher quality, even with half modeled blacked out interiors. start with the wasp.  (cars)
	1. name all the game objects accordingly
	2. make an ambient occlusion texture.
	3. make seperate materials for headlights and backlights
	4. make blacked out blocky interiors.
	5. make bespoke wheels with brakes and very basic suspension.
	6. make side mirrors.
	7. actually model the innards of the cars like the radiators and engine headers. but only stuff visible from the outside. kinda.
	8. Uv unwrap the cars onto 1 texture. to easily add liveries if needed.
	9. shape key a simple damage system, for front, side left and right and back and top damage.
	10. make bespoke audio clips for each car.
	11. use the ambient occlusion texture, invert it, and map it to the specular map.
	12. animate wings.
	13. use autodesk image modeler to setup the modeling enviorment, so you dont need to rely on low res blueprints anymore. yay.
	
16. add new cars like the: (cars)
	1. seat leon -> spanish revolver.
	2. agera R -> ghost
	   
17. make a new map, check [[map to make]] (world)
18. add dirt particles, and fake dirt on the car using decals. (VFX)

---
## ways to go about finishing those to dos:

- separate the points into different categories that are finished and worked on asynchronously. meaning you can work on 1 of each category at the same time.

what are the categories:
- physics (P)
- visual and audio effects (VFX)
- UI (UI)
- environment art and models (world)
- car models (cars)
- AI (AI)
- misc (misc)

---

## todos in the game itself:

things to do to actually get to the final product.

- before you even start on the project you need to start modeling the map itself. so you'll have something to occupy you while you tediously move things around, and something to motivate you aswell.
- you'll then have to migrate everything about this game to the new map
- you replace the main menu with a start screen
- and add the option to switch from the dev to player mode which will change the functionality of the debug menu.
- re modeling the cars wouldn't be the utmost priority, but something you put on the backburner so that when the game it ultimately done, you'd have a huge chunk of the cars facelifted. but I do advice to make a blockout of the cars first so you can build events around that.
- when the layout of the map is done and all the roads are set and the terrain is being filled out, make as much events as possible.
- when you have enough events we will now work on the progression. you'll add a money mechanic, a streak system, add all the functionality to the hyperdrive menu, and add the ability to lock and unlock cars accordingly.
- now all thats left in this phase is to make the boss event, the one boss event, the agera r / ghost.
- now that the skeleton of the game is done, all you need is alot and ALOT of polish. finish up the map, finish up the cars, tidy up the events, fix the bugs, make the ui more appealing, add quality of life improvements and make the game public ready.

so the current plan is:
1. map
2. events
3. progression
4. cars
5. polish


---
### physics plan:

making it easier to evolve the physics model
#### replacing the springs

- make the spring force code area a toggle, this will make the car lie flat on the ground if turned off
- add the 6dof nodes and give them their rigidbodies and a cylinder mesh.
- make them work as springs on the wasp first.
- add them to every car.
- once that is done connect the data sheet values to the springs.
- remove the old spring code. and the toggle.

#### giving the wheels their rigidbody privileges

- connect the rigidbodies to main script
- in the drivetrain section, make it so it adds the weight of the drivetrain as inertia to the appropriate rigidbodies, and more weight if the clutch is engaged. do this to the x axis.
- add the engine power as torque to the appropriate wheels. multiplied by the wheel radius.
- same for braking.
- remove all the excess code.
- do it to all drivetrain types.
- remove all access nodes.
- do this to all cars.

#### make the traction code work with the new rigidbody wheels

