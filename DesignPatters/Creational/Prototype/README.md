<h1>Prototype:</h1>

<h2>Problem:</h2>

Imagine you have an object and you need a copy of it. You could create it and copy all properties, but in this case you could have a problem, because the private properties won't be visible from outside of the object itself. Also with this approach since you have to know the object's class to create a duplicate, your code becomes dependent on that class, but if this is not enough somethimes you only know the interface that the object follows, but not its concrete class, for example, a parameter in a method accpets any objects that follow some interface.

<h2>Solution:</h2>

The solution here is simple, just delegate the cloning process to the actual objects that are being cloned. 

![plot](./images/structure-3.png)