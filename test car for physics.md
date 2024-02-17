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