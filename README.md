# C++ Gravity Simulator
Creating an N-body gravity simulator in C++, with OpenGL and Vulkan visualisation

## Basic Gravity Simulation

Creating objects with attributes:
```
PhysicsObject object1;
object1.mass = 10;         // kg
object1.p = {0, 0, 10};    // position
object1.v = {0, 2, 2};     // velocity
```

Calculate the forces between objects using the Gravitational Force equation:

$$F=\frac{GMm}{r^2}$$
