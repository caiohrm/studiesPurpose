<h1>Abstract Factory</h1>

Abstract Factory lets you produce familes of related objects without specifying concrete classes, in this case you basically are going to create an interface with the methods you need your classes to implement, and the classes will implement each method with theyrs specificity, so in this case when someone needs to call an specific method for some class it wont need to know the class type just the interface

Ex: 

Imagine you have a factory that produces diferent types of chairs, tables, coffe center...

In this case how can we deal with the problem of having diferent classes of chairs, tables, coffe center...? We should only create an Interface for each type of furniture (**IChair**,**ITable**,**ICoffeCenter**...), **so in this case if we have a diferent type of chair we just need to implement the IChair interface.**

**But what if now we need a class that creates always the same type of furniture ?**

Ex: I'm going to need to create chairs and tables with the same caracteristics, how can I ensure that this will happen?

In this case I'll need to create a Interface for each kind of furniture I need to create (**IFurnitureFactory**), so everytime that I need a Vintage chair I can just call the interface IFurnitureFactory instead of the class (ModernFactory, VintageFactory...) **and the method itself its going to return an interface IChair for me**, in this case the client don't need to know the type of the class to call, he just need to ask for the chair:


![plot](./images/structure.png)