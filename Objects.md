# OBJECT ORIENTED
* A program is made up of many cooperating objects
* Instead of being the "whole program" - each object is a little
"island" within the program and cooperatively working with other objects.
* A program is made up of one or more objects working together - objects
make use of each other's capabilities

## Object
* An object is a bit of self-contained Code and Data
* A key aspect of the Object approach is to break the problem into smaller
understandable parts (divide and conquer)
* Objects have boundaries that allow us to ignore un-needed detail
* We have been using objects all along: String Objects, Integer Objects,
Dictionary Objects, List Objects...
* Objects hide detail - the allow the "rest of the program" to ignore the
detail about "us"

<dl>
  <dt>Class</dt>
  <dd>A template</dd>
  <dt>Method or Message</dt>
  <dd>A defined capability of a class</dd>
  <dt>Field or attribute</dt>
  <dd>A bit of data in a class</dd>
  <dt>Object or Instance</dt>
  <dd>A particular instance of a class</dd>
  <dt>Attribute</dt>
  <dd>A variable within a class</dd>       
  <dt>Constructor</dt>
  <dd>Code that runs when an object is created</dd>
  <dt>Inheritance</dt>
  <dd>The ability to extend a class to make a new class</dd>
</dl>

**Terminology: Class**  
Defines the abstract characteristics of a thing (object), including the thing's characteristics (its attributes, fields or properties) and the thing's behaviors (the thing it can do, or methods, operations or features). One might say that a class is a blueprint or factory that describes the nature of something. For example, the class Dog would consist of traits shared by all dogs, such as breed and fur color (characteristics), and the ability to bark and sit (behaviors)

**Terminology: Instance**  
One can have an instance of a class or a particular object. The instance is the actual object created at runtime. In programmer jargon, the Lassie object is an instance of the Dog class. The set of values of the attributes of a particular object is called its state. The object consists of a state and the behavior that's defined int he object's class. 

**Terminology: Method**  
An object's abilities. In language, methods are verbs. Lassie, being a Dog, has the ability to bark. So bark() is one of Lassie's methods. She may have other methods as well, for example sit() or eat() or walk() or save_timmy(). Within the program, using a method usually affects only one particular object; all Dogs can bark, but you need only one particular dog to do the barking.

## OBJECT LIFECYCLE
* Objects are created, used and discarded
* We have special blocks of code (methods) that get called
	* At the moment of creation (constructor)
	* At the moment of destruction (destructor)
* Constructors are used a lot
* Destructors are seldom used
* The primary purpose of the constructor is to set up some instance variables to have the proper initial values when the object is created

## MANY INSTANCES
* We can create lots of objects - the class is the template for the object
* We can store each distinct object in its own variable
* We call this having multiple instances of the same class
* Each instance has its own copy of the instance variable
* Constructors can have additional parameters. These can be used to set up instance variables for the particular instance of the class (i.e., for the particular object)

## INHERITANCE
* When we make a new class - we can reuse an existing class and inherit all the capabilities of an existing class and then add our own little bit to make our new class
* Another form of store and reuse
* Write once - reuse many times
* The new class (child) has all the capabilities of the old class (parent) - and then some more
* 'Subclasses' are more specialized versions of a class, which inherit attributes and behaviors from their parents classes and can introduce their own
