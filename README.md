# Personal Tracker

Welcome to the github page for HyperBlock! This is a development project that aims to create a 3D voxel based game that takes place in an alternative spacial structure/dimension, called hyperbolic space.

Having a different strucutre, this space has many odd qualities: parallel lines always drift apart, squares no longer have 90 degree angles in their corners, in fact, now pentagons can be made to have 90 degree corners instead, space expands exponentially faster the further you go, making it easy to get lost.

Due to these effects, building and navigating the space itself becomes a unique challenge!

## Features

Development in a new spatial structure is no easy task. Basic storage, tracking and calculations that are usually assumed now break down. 

Graphics is a major hurdle. There is a reason why you can't imagine a square with straight lines to have anything but 90 degree corners; this type of space is not compatible with ours. To allow any type of rendering, a projection of this space is used. This is similar to spherical geometry: to have a flat map of the Earth, we have to project the 3D spherical surface onto a flat surface. This projection is never an accurate representation, and is always accompanied by distortions. A similar effect happens with hyperbolic geometry (only instead, it is projected into a 3D space).

Below is a 2D analog of hyperbolic space projected in a way that we could visualize on a flat surface. Square edges are straight lines of equal length; however, they shrink and curve the far from the centre point, similar to how a map curves and grows toward the poles.

<img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/3844d843-6608-44f0-80ef-2454016ee2a4" />

An alternative spatial coordinate system is also required. In hyperbolic space, a square can be made to have 72 degree corners, like in the image above. This is the only way to tile squares into a grid into this example of space.

But how could a coordinate system exist in this space? If lets say we assumed a square was a room in a house, it wouldn't take long before realizing what were once floors are now walls, giving an Escher-esque feeling.

<img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/a7ec6343-3b51-4f36-a93f-9b4edd1a003a" />

So in this case, what is horizontal or vertical? What do we use as an "x-axis" and "y-axis" if these core concepts have broken down?

And like mentioned before, parallel lines drift apart, meaning that any line as a reference axis is bound to drift in "direction". See below, an example of the parallel walls of a square, where above and below, an infinite amount of space rapidly expands. 

<img width="960" height="960" alt="image" src="https://github.com/user-attachments/assets/93043f30-f6ec-4730-99da-0c346f307b79" />

The solution is instead to codified symmetries about an origin square defined by a Coxeter System, a more abstract representation useful for understanding geometric structures and patterns.

For example, the position of the green fish below would be defined as a reflection about the red line with respect to the red fish. We could call this reflection "A"

<img width="421" height="416" alt="image" src="https://github.com/user-attachments/assets/46bd1946-a1a7-45fb-98d6-4ffed3015f09" />

The coordinate system would, instead of adding distance along an x, y, or z axis, add consecutive reflections along face "A", "B", "C", for example, and be rather than be understood as distances along multiple axis like (x: 32.0, y: 42.0, z: 0.0), they would be codified as a series of reflections along multiple faces like "ABBCBA", which would represent a position requiring 6 reflections to get to.

## Update Vlogs

https://www.youtube.com/watch?v=l48AZWLv4Ys

https://www.youtube.com/watch?v=8Jr8QMm3F4U

https://www.youtube.com/watch?v=NzK0MCwgLE8



