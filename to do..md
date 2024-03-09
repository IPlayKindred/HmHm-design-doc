no need to them at order, ofc that depends on each item in the list.

dont push yourself too hard.

1. cut all the engine audio clips to 1 seconds or less. which if all the cars are factored in, each with separate and unique engine audio, it will add to less than 40mbs.
2. Add a test car and test all the new physics stuff on it like 6dof joints. [[test car for physics]]
3. remove all the old maps. for multiple reasons.
4. make the awareness raycast rotate around to the car to emulate multiple raycasts without the increased performance requirements.
5. make the camera rigidbody and use 6dof joint to attach it to the car.
	- by the camera I mean add a misc rigid body to the car itself with a 6dof, to every car. and just make the camera copy its transform.
6. move the physics code to C#, but only the physics code and nothing else.
7. add a lap system to the event manager and event data.
8. different camera option, only add a bumper camera.
9. control mapping option.
10. save data for the options.
11. smoke particles.
12. skid marks.
13. brake and headlights.
14. Complete the car variable editor, the weight, forward friction and assists tab.
15. remake all the cars to be alot, and I mean alot more higher quality, even with half modeled blacked out interiors. start with the wasp. 
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
	
16. add new cars like the:
	1. seat leon -> spanish revolver.
	2. agera R -> ghost
	   
17. make a new map, check [[what maps to make]]
18. add dirt particles, and fake dirt on the car using decals. 