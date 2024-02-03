# C++ Gravity Simulator
Creating an N-body gravity simulator in C++, with OpenGL and Vulkan visualisation

## Basic Gravity Simulation

Creating objects with attributes:
```c++
PhysicsObject object1;
object1.mass = 10;         // kg
object1.p = {0, 0, 10};    // position
object1.v = {0, 2, 2};     // velocity
```

Calculate the forces between objects using the Gravitational Force equation:

$$F=\frac{GMm}{r^2}$$

Apply the force from all other objects to get the total force:

```c++
for(int i = 0; i < numOfObjects; i++)
{
        for(int j = 0; j < numOfObjects; j++)
        {
                force += (G * object1.mass * object2.mass) / (distance * distance);
        }
        object1.a = force / object1.mass
}
```
