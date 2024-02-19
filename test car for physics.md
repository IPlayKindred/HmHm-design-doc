before starting you should wait for this first.
1. jolt for godot version 4.3
2. complete version godot 4.3

the car should have no separated body parts, its all one objects. except for the windows.

what should the car be? it'll be an early version of the wasp facelift.

the car should probably have a copy of the main car_physics.gd script

and every single idea should be tested on it.

like:
1. 6dof and rigidbodies for each wheel.
2. 2 rigidbodies to represent the engine and the rest of the drivetrain, both attached through a 6dof.
3. change and adapt the bespoke script for the new changes in physics.
4. polish and make everything at tip top shape so you can change all the cars to that.
5. use hinge joints for steering and use the wheel rigidbody forward dir to calculate slip and angle and slip ratio.
6. an energy recovery system (ers):
	this acts in the same way as burst nitrous, but the power of the burst is in how much energy is in the system, you gain energy by braking, the higher your speed while breaking, the more speed you lose, the bigger the energy, and the bigger the burst.
	
	it also works in a way that energy gain is exponential, the difference between 150 and 160 is much much more than 90 and 100, even tho they're both 10 apart.
	
	other ways to recover energy, is the time the car go down from air, the faster the  descent the better, also the higher the slip ratio, the more energy the ers system gains, as to compensate for the lost grip.
	
	the more downforce there is, the more energy is gained. 