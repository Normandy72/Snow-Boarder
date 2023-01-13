# ~ Unity ~
## Add Cinemachine
1. Add the Package Manager window.
2. Find and install Cinemachine.
3. Add a Virtual Camera.
4. Point it to follow the ball.
5. Change the Screen X value to show more of wants to come.

## Surface Effector 2D
1. Add Surface Effector 2D to main layout
2. In Edge Collider mark 'Used by Effector'

## Particle System Component
* Particle System is a Component added to a Game Object.
* We use Modules for controlling behaviour.

***
# ~ C# ~
## Organising Code
* The more code we have, the higher likelihood of conflicts between names and behaviours. Especially on multi-person projects. E.g. Programmer 1 working on player uses "Movement" method but Programmer 2 working on enemy also uses "Movement" method.
* So in C# our code is grouped with a particular structure to reduce conflicts.
```
namespace UnityEngine
    class OurClass
        SomeMethod()
            statementA;
            statementB;
```
## Creating A Delay
* There are 2 useful approaches to "waiting a moment":
    * Invoke,
    * Coroutines.
* Invoke is a bit easier to understand but not as powerful.

## Using Invoke()
When we call `Invoke()` we need to pass in the name of the method we want to call after a delay, as well as how long the delay is.

`Invoke("NameOfMethod", delay);`