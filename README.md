Download link :https://programming.engineering/product/homework-03-gt-night-at-six-flags/


# Homework-03-GT-Night-at-Six-Flags
Homework 03 – GT Night at Six Flags
Problem Description

You have been hired by Six Flags to deliver the next big ride tracking system. The roller coasters and trolleys have been bought – your co-workers are just waiting for the code! And so, you set out to amusement parks to learn more about how you should implement the system.

Solution Description

You will create three classes: Ride.java, RollerCoaster.java, and Trolley.java. In this assignment, we use the following definitions:

A “stop” refers to an individual destination along the ride.

For roller coasters, a “stop” is synonymous with a “run”.

A “run” consists of stop(s) and refers to an entire loop on the ride.

For roller coasters, a run consists of one stop.

For trolleys, a run may consist of multiple stops.

Notes:

All variables should be inaccessible from other classes and require an instance to be accessed through, unless specified otherwise.

All methods should be accessible from everywhere and must require an instance to be accessed through, unless specified otherwise.

Use constructor and method chaining whenever possible! Ensure that your constructor chaining helps you minimize code repetition and maximize code reuse!

Helper methods with appropriate visibility are optional.

Make sure to add Javadoc comments to your methods and classes!

You must not write getters or setters for Ride.java, RollerCoaster.java, and Trolley.java. This assignment can be completed without the use of any getters or setters.

Constructors must deep copy any mutable arguments to the corresponding instance field.

Ride.java

This class represents any amusement park ride. Ride should never be instantiated. Instead, it should only serve as a superclass for more specific rides.

Variables:

For fields in Ride, use the most restrictive visibility modifier that allows the fields to be accessible from any subclass.

String id – the identifier of this ride

This variable should be immutable after construction of an instance.

double earnings – the total amount of money this ride has earned, always initially 0

int runsSinceInspection – the number of runs this ride has completed since the most recent inspection

String[] passengers – the names of passengers aboard this ride.

Constructors:

A constructor that takes in id, runsSinceInspection, and passengers.

Note: The passengers argument array must be deep copied to the corresponding instance field. This means that you should not simply copy the reference of the input array and assign it to the instance field.

A constructor that takes in id, passengers, and sets runsSinceInspection to 0.

Assume all constructor inputs are valid.

Methods:

canRun

Takes in an int number of runs and returns a boolean that represents whether the ride

can complete that number of runs without needing an inspection.

This method should not have an implementation in the Ride class.

Hint: What keyword allows us to declare a method in a class without providing an implementation?

inspectRide

Takes in a String[] that represents different components of the ride.

Resets runsSinceInspection to 0 if the ride passes inspection and returns true.

Returns false if the ride does not pass inspection.

This method should not have an implementation in the Ride class.

Hint: What keyword allows us to declare a method in a class without providing an implementation?

costPerPassenger

Takes in an int number of stops and returns a double representing the cost for the passenger to ride the specified number of stops.

This method should not have an implementation in the Ride class.

Hint: What keyword allows us to declare a method in a class without providing an implementation?

addPassengers

Takes in an int number of stops and a String[] of passenger names.

Returns true if all new passengers can fit on the ride and the ride can travel the given number of stops without an inspection, and false otherwise.

This method should not have an implementation in the Ride class.

Hint: What keyword allows us to declare a method in a class without providing an implementation?

getPassengerList

Returns a list of passengers as a String in the specified format.

Only one name should be on a line.

Only non-null elements should be listed.

No leading nor trailing whitespace on each line.

Assume that each name does not have trailing or leading whitespace.

This method will be very helpful when testing the addition and removal of passengers from the ride.
