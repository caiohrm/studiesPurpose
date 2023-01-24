<h1>Hexagonal architecture:</h1>

<h2>Principles:</h2>

- This model is based on ports and adapters

- Its based on the Idea that the architecture should be focused at the business behavior and not in the database, comunication etc...

<h2>Ports:</h2>

The ports are the gateway comunication between the certer of the hexagon with the right and legt sides with the external side

<h2>Adapters:</h2>

The adapters are the ports users. For each port that your hexagon has, one adaptor must be created, so in this case you have the freedon to change it and and delete it dynamically.

<h2>Positive sides:</h2>

- Independent external services 
- The possibility to delay some technical decisions
- You can create and change the adaptors
- Easier to test the application
- Easy to change the technology

<h2>Negative sides:</h2>

- More complexity (You need to build more layers)
- Higher cost to build and mantain
- No guidance in how to organize the code (directory, layers...)

![plot](./images/100-explicit-architecture-svg.png.webp)