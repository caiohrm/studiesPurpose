<h1>Clean architecture</h1>

<h2>Here it doesn't say how to write a code architecture, but it gives you some principles to write a good architeture</h2>

- Created by Robert C. Martin in 2012

- Define the separation of responsabilites at the architecture

- Based in rules to create a flow of dependencies where you can build the architecture with low coupling

<h2>Principles</h2>

- Dependence rule (The higher part of the architecture will depend on the lower part, but never the other way)

- Abstraction principle (In this principle we are saying that we should keep the object as abstract as possible)

- [SOLID](../../SOLID/) (This is the most important principle for this architecture)

- Reuse/Release equivalence principle REP (if the objects need to be changed together it needs to be released together )

- Common closure princile CCP (If the objects needs to be changed together it needs to together so you don't loose anything )

- Common reuse principle CRP (Don't implement dependencies that you wont use it)

- Acyclic dependency principle ADP (Don't implement any dependency where they will need each other, in this case you should use some design patters as an [Adapter](../../DesignPatters/Structural/Adapter/) for example )

- Stable dependency principle SDP (The least stable component should depend on the most stable component and never the other way)

- Stable Abstractions Principle SAP (The most stable component should be the most abstract components, and it should have the minimun of depence)




![plot](./images/CleanArchitecture.jpg)