this is to make the map making process easier. since its really mind consuming and alot of things get overlooked.

### THE DON'Ts

1. Focus on the details instead of silhouettes, especially very early on when it the silhouettes weren't even defined.
2. Go in without establishing the layout of the road first, weather its organically building up on the roads in blender and testing them in blender and/or drawing them on a piece of paper beforehand.
3. go in without reference images and concept art, these are extremely important and should probably be the utmost priority, cuz they dictate the entire map.
4. finishing the road and terrain without making it fun to begin with.
5. using final textures immediately instead of testing it all out with grid textures.
6. Go in to the terrain filling phase without polishing and finalizing the roads, since doing so will make changes to said roads extremely hard to implement.
7. going into the terrain filling phase without separating the roads into chunks. the smaller the better, but don't cut too small.
8. rush the terrain filling process, which leaves jagged edges and awful topology.
9. skipping the blockout phase.
10. not using reference or concept art for the blockout phase.
11. utilize the verticality of the setting as much as possible, the more vertical the setting looks, the more roads should utilize that.

---


### GET REFERENCES

in the triple digits, the more, the better organized the better.

---


### SKETCH (for concept art) and LAYOUT (for actual map)

Block in simple big shapes first using the already existing reference images.

Iterate on the sketch, don't feel bad if you need to make a couple of iterations on it. Take your time.


using the sketch, make up the layout of the roads.

make a version where you plan out all the roads.
then connect the intersections and whatnot and send it out to godot to test it.

then go back to the pre modified splines and adjust.
rinse and repeat until you have the main road network.

then you'd have the main road network. add more roads, shortcuts, open areas, vertical areas on building and stuff, bridges. to make it more fun and interesting.

what to add to spice it up:
1. a backup road going around a tight turn to act as a safety net.
2. jumps going to the roof of buildings
3. the roofs of said buildings having their own road network that connect back to the road through jumps.
4. hangers, garages, dock storage areas and parking lots for indoor areas
5. underground tunnels.
6. a secondary road around long straights that snakes around it and is broken up by jumps. that connect to other anomalies like bridges and roof, etc, etc.

---


### PAINT

Plan out the color pallet beforehand. Using multiple color pallets if needed. Using the reference images to help with the color picking.

Using adobe colors. And reference images as suggested before.

big shapes first, then fill in detail.

---


### RENDER

Don't go too overboard. Try to be as quick as possible, just iterate, what you need is time and patience, this piece will be used as a reference and a testing piece for the next concept artworks.

---


### MAKE MORE CONCEPT ART

Using your new found knowledge on how to draw concept art for the specific map, Just don't be obsessed with making good art at this stage.

Concept art should solve problems like what the textures would look like, what props are placed where, what the hierarchy would be, basically taking the painted piece that was made just to look good, and making it as technical and as helpful as possible.

fill each part of the map with appropriate concept art.

Come up with the cool ideas in this stage, experiment as much as you can, you didn't block out anything yet, and better yet, if you did make the road related to track, you could do that as well.

Closing doors, sit down with yourself after every brainstorming session, see the ideas you liked and the ones you didn’t, the ones you didn't, close the door on and expand on the ones you did like, like evolution.

Avoid grand reveals for yourself. Show your work to yourself as early and as often.

Make a layer in each krita file. That just outlines the geometric shapes so it's easier to model.

Numbering the outlines based on priority so it can be followed even easier on the modeling process.

---


### BLOCKOUTS

Make a plan on what the map layout would look like, using the before talked about references to help you as well as the concept art, make it as concise and detailed as it needs to be, leaving as little room for interpretation as possible. So the modeling process isn't as tedious.

The plan should also be as sketch-less as possible, like using sketching ofc, but keep it at a minimum.

Again, iterate on the sketches as much as possible.

Make the road and fill out the terrain.

Using the plan you’ll need to block out the geometry in the map blend file. Use basic shapes, prioritizing the big shapes first, then honing in and using smaller and smaller basic shapes.

When you can’t go any further with basic shapes, you’ll then need to move on to the next step.

---


### MODEL AND REFINE THE BASE MODEL

Using the blockouts you’ll then make a new mesh modeled around them. This will be tough, use the blockouts as much as you can.

It’ll take time and a lot of patience, use the references and the plan and the outlined geometry on the concept images.

probably the most tedious part of the process.

Remove unneeded geometry, and try to refine as much as possible, keeping it somewhat simple. So it can be painted over.

The less geometry the better.

---

### PAINT OVER USING THE TEXTURE PAINT TOOLS AND USE THE CONCEPT ART

Use the blender texture painting preset, use stencil tools, use the reference images, try to bake as much of the lighting in as possible, mainly ambient lighting.

Keep this part as detailed as you possibly can. The more refinement and time you give it the better.

This is basically the process where everything comes together. Have fun.

Once you’re done, save the textures and refine them in krita.

Then export them back into the blend file. So it can be exported to godot using the gltf file format.

---
### GET READY TO EXPORT

Calculate geometry origins. Save all the textures from krita into a file. Name all the objects accordingly, patch them into collections so they can be exported into separate gltf files.

Export them, name the gltf files and put them neatly in the same file.

---

### ASSEMBLE IN GODOT

Basically as the title says, assemble them, give them names, make the collisions for them, yata yata, and enjoy, you’re done. Have fun with the map.

---

so yeah, that's the plan for making the maps on a more technical level.
