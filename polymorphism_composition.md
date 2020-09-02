Polymorphism & Composition Homework - Quiz
Polymorphism
What does the word 'polymorphism' mean?
Many forms.


What does it mean when we apply polymorphism to OO design? Give a simple Java example.
We wrap two or more different objects with a type, or tag, in order to reduce the amount of functions that we have to write.


What can we use to implement polymorphism in Java?
We can give our classes the same super class, or an interface.


How many 'forms' can an object take when using polymorphism?
It can have only one parent superclass (though if that has parent class too then it can be treated as that class too), but many interfaces.


Give an example of when you could use polymorphism.

abstract class Car();
class PetrolCar extends Car();
class ElectricCar extends Car();

Public String whatCar(Car car) {
    return "This car runs on " + car.getFuelType;
}

electricCar.whatCar();


Composition and Aggregation
What do we mean by 'composition' in reference to object-oriented programming?
An object that relies on another object for it's existance is composed of that object.


When would you use composition? Provide a simple example in Java.
A guitar needs various things, such as a neck and a body.

class Neck {
    private String material;
    private int length;
}

class Body {
    private String material;
    private String pickups;
}

class Guitar {
    private Neck neck;
    private Body body;

    public Guitar() {
        this.neck = new Neck();
        this.body = new Body();
    }
}

Give a difference between composition and aggregation?
In aggregation, the objects involved in the composition of an other object can survive independently of the singular object.


What is/are the advantage(s) of using composition/aggregation?
When inheriting attributes or functions, composition/aggregation allows us the luxury of many inheritances, wheras we are limited to one  when inheriting from a superclass.


When using composition, when an object is destroyed, what happens to all the objects it is composed of?
They are destroyed too.


When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?
They can survive independently.
