Open close Principle
--------------------
Software Entities(<b>CLASSES, METHODS, MODULES, etc. </b>) should be open for extension, closed for modification.

In the example, we have common fields (subscriberId, phoneNumber, address, baseRate) and a common function (calculateBill) in case of phone and internet subscriber.
Instead of keeping all the fields in both of classes PhoneSubscriber and ISPSubscriber, created abstract class called Subscribers with all the common fields
where all the fields are protected and abstract method. So, PhoneSubscriber and ISPSubscriber is extending the subscriber class, but it can't modify
the fields and implement the calculateBill according to the usage.