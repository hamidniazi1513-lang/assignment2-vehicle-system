Vehicle Management System

Object-Oriented Programming — Inheritance and Abstraction

 Project Overview
This project was created to practice and demonstrate the main concepts of Object-Oriented Programming (OOP) in Java. The goal of the project is to build a simple Vehicle Management System that shows how inheritance, abstraction, and object relationships work in a real-world style example.
In this system, all vehicles share common characteristics, such as brand and year, which are defined in an abstract Vehicle class. Specific vehicle types like Car, Motorcycle, and Truck extend this class and provide their own behavior. A separate Driver class is used to represent drivers and show how vehicles can be associated with drivers.

 Class Hierarchy
At the top of the hierarchy is the abstract Vehicle class. It contains shared fields and methods that are common to all vehicles, as well as abstract methods that must be implemented by subclasses.
* Vehicle (abstract class)
  * Fields: brand, year, driver
  * Abstract methods: startEngine(), stopEngine()
  * Concrete method: displayInfo()
The following classes extend the Vehicle class:
* Car – represents a car with additional details such as number of doors and fuel type
* Motorcycle – represents a motorcycle and includes information about a sidecar
* Truck – represents a truck with load capacity and number of axles
Each subclass uses constructor chaining with super() and overrides the engine methods to provide behavior specific to that type of vehicle.
The Driver class is independent from the vehicle hierarchy and stores driver information such as name and license number. One driver can be associated with multiple vehicles.
 Instructions to Compile and Run
To compile and run the program, navigate to the src folder and execute the following commands:

javac *.java
java Main


 Reflection
Using inheritance made the design of this project much simpler because common properties and methods only needed to be written once in the Vehicle class. This helped keep the code organized and reduced repetition.
Method overriding allowed each vehicle type to have its own engine behavior while still being handled through the same Vehicle reference in the main program. One of the challenges I faced was choosing the correct access modifiers, especially deciding when to use protected instead of private so that subclasses could still access necessary data without breaking encapsulation.

