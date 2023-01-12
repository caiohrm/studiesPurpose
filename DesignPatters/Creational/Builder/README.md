<h1>Builder:</h1>

<h2>Problem:</h2>
Imagine a complex object that requires laborious, step-by-step initialization of many fields and nested objects. Such initialization code is usually buried inside a monstrous constructor with lots of parameters. Or even worse: scattered all over the client code.


 Lets think about how to create a house in this case, we need to build at least four walls, windows and a dor, but what if we whant to build a bigger wall and a bigger window, what about if we whant a backyard?

The simplest solution is to extend the base **House** and create a set of subclasses to cover all the combinations of the parameters. But eventually you'll end up with a considerable number of subclasses. Any new parameter, such as the backyard, will require growing this hierarchy even more 


The other approach it's to create a giant constructor right in the base **House** class with all possible parameters that control the house object, but it creates another problem, in most cases most of the parameters will be unused, making the constructor calls pretty ugly.


<h3>Solution:</h3>


The **Builder** pattern suggests that you extract the object construction code out its own class and move it to separate objects called builders. In this case you'll create a serie of steps such as **BuildWalls, BuildDoors and BuildBackYard**. The importante part is that you don't need to call all of the steps. You call only those steps that are necessary for producing a particular configuration of an object.


 Ok but what if we whant to build wall of wood, rock, diamant... In this case we can just add a parameter to define the type of material.

<h3>Director</h3>


The director it's not necessary but if you whant you can create a director so it will have all the steps to execute the building steps, while the builder provider the implementation for those steps. this is good so you can reuse the routines across your program.


![plot](./images/structure-2.png)
