<h1>Adapter:</h1>

<h2>Problem:</h2>

Imagine you have an app that downloads data from multiple apis in the xml format, and after some time you need to connect with an api that works with data in JSON format.

You could change the library to work with xml. However, this might break some existing code that relies on the library. Or worse, you might not have access to the library's source code in first place, making it impossible.

<h2>Solution:</h2>

You can create an adapter. This is a special object that converts the interface of one object so that another object can undertand it.

1- The adatper gets an interface, compatible with one of existing objects.

2- Using interface, the existing object can safely call the adapter's methods.

3- Upon receiving a call, the adapter passes the request to the second object, but in a format and order that the second object expects.

Sometimes it's possible to create a two-way adapter that can convert the calls in both directions.

