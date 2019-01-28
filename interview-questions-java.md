Interview Questions -- Java
==========================

**What is Java?**

Java is a high-level programming language originally developed by Sun Microsystems and released in 1995. Java runs on a variety of platforms, such as Windows, Mac OS, and the various versions of UNIX. Java is fast, secure, and reliable.

**What is JDK stands for and what are the components of JDK?**

**JDK:** Java Development Kit

**Components:**

-   The Runtime Interpreter,
-   The Compiler,
-   The Applet Viewer,
-   The Debugger,
-   The Class File Disassembler,
-   The Header and Stub File Generator,
-   The Documentation Generator,
-   Applet Demos,
-   API Source Code.

**What is IDE stands for and what IDE are we going to use?**

**IDE:** Integrated Development Environment, Eclipse/IntelliJ IDEA.

**Explain the entire life cycle of Java?**

1.  A Java program is written using either a Text Editor like Textpad or an IDE like Eclipse and is saved as a `.java` file. (Program.java)
2.  The `.java` file is then compiled using Java compiler and a `.class` file is obtained from it. (Program.class)
3.  The `.class` file is now portable and can be used to run this Java program in any platform.
4.  Class file (Program.class) is interpreted by the JVM installed on a particular platform. JVM is part of the JRE software.

**What is RAM stands for and what are the segments in RAM?**

**RAM:** Random Access Memory.

Segments in RAM:

-   Data
-   BSS (Basic Service Set)
-   Stack
-   Heap

**What is JVM stands for?**

**JVM:** Java Virtual Machine, enables a computer to run a Java program.

**Write about java history, like when it was invented and now which company it belongs to?**

James Gosling, Mike Sheridan, and Patrick Naughton initiated the Java language project in June 1991. Now it belongs to Oracle.

**Write the command to check if java exist and it's version in your machine.**

`java -version`

**What version of java are we using currently?**

```
java version "1.8.0\_151"
Java(TM) SE Runtime Environment (build 1.8.0\_151-b12)
Java HotSpot(TM) 64-Bit Server VM (build 25.151-b12, mixed mode)
```

**What is difference between Path and Classpath?**

Path and Classpath are operating system level environment variables. *Path* defines where the system can find the executables(.exe) files and *classpath* is used to specify the location of .class files.

**What is Class in java?**

Class is a blueprint of an object. It describes the behavior and state that the object of its type support.

**What is Object in java?**

Object is an instance of a class. It has some states and behaviors.

**What is the relationship between a class and an object?**

A class is a blueprint but when it needs to come into existence, it uses objects. So they are interdependent. 

**Why do we need at least one "main" method in java to run the application?**

By providing at least one main method java compiler gets the starting point to run the application. Otherwise it cannot run.

**Is Java Strongly Typed Language?**

Yes.

**Is Java case sensitive?**

Yes.

**Is Java all about class and object?**

Yes.

**What "new" keyword does?**

It is a Java reserved keyword which is used to create a new object from an existing class.

**What is variable? What are different Type of variables? Outlined them all.**

Variable is name of *reserved area allocated in the memory*. A named memory location to store the temporary data within a program, It is a combination of "vary + able" that means its value can be changed.

There are three types of variables.

-   **Local variable** --- are declared in methods or blocks.
-   **Instance variable** --- are the class variables but are declared outside the method and block.
-   **﻿Class variable** --- are those class variables which are defined with the static word. These cannot be local.

**Difference between declaring and initializing variable?**

-   **Declaring variable** means a variable gets a variable name and a variable type.
-   **Initializing variable** means to give a value to the variable.

**What are the primitive data types in Java?**

There are **8 primitive types** of data built into the Java language.

-   byte, short, int, long, float, double, boolean, char.
-   primitive variables store primitive values.

**What are the reference data types in Java?**

Reference types are any instantiable class as well as arrays.

-   String, Scanner, Random, Die, int[], String[], etc.
-   Reference variables store addresses.

**How are Java primitives and objects stored in memory?**

In Java,

-   value types (primitives) are stored on the stack.
-   reference types are stored on the heap.

**Different type of method?**

There are two types of methods.

-   **Void**** method** which does not return anything.
-   **Return method** which returns some values.

**Outline Access Specifier**

There are four access specifier in java.

-   **Public** --- public access modifier is accessible everywhere.
-   **Private** --- private access modifier is accessible only within the class.
-   **Protected** --- protected modifier is accessible within the package, outside of the package but through Inheritance.
-   **Default** --- if we don't specify any modifier then it is treated as the default, can be accessed only within the package.

**What is the difference between private and public modifier?**

A public member is a member of a class that can be accessed by anyone. A private member is a member of a class that can only be accessed by other members of the class.

An access specifier determines who has access to the members that follow the specifier.

**Why Generics are used in Java?**

Generics provide compile-time type safety that allows programmers to catch invalid types at compile time. Java Generic methods and generic classes enable programmers to specify, with a single method declaration, a set of related methods or, with a single class declaration, a set of related types.

**What is dot operator?**

The dot operator(.) is used to access the instance variables and methods of class objects. It is also used to access classes and sub-packages from a package.

**Is java has automatic garbage collector?**

Yes.

**What is Constructor?**

It initializes a new object of a class. It does not have a return type. It has the same name as the class it belongs to.

**Can you have multiple Constructor in one class?**

Yes. A class can have multiple constructors, each with a different number or type of argument.

**If there is no Constructor declared, which one it is called during the Object creation?**

The default constructor.

**What is "this" keyword in java?**

Keyword *THIS* is a reference variable in Java that refers to the current object.

-   It can be used to refer instance variable of the current class.
-   It can be used to invoke or initiate current class constructor.

**What is Abstraction?**

It is a feature of OOP. It is an implementation hiding process.

**What is Interface?**

It is a blueprint of a class. It has abstract methods only.

**What is Abstract class?**

It contains both abstract methods and concrete methods.

**What is the difference between Interface and Abstract class?**

Interface cannot have implemented methods but abstract class can have implemented methods.

**Can you instantiate Interface and Abstract class?**

No, only concrete class can be instantiated.

**Can an Interface extend another Interface?**

A Java class can only extend one parent class. *Multiple* inheritance is not allowed. Interfaces are not classes, however, and an interface can extend more than one parent interface. The extends keyword is used once, and the parent interfaces are declared in a comma-separated list.

**Can Abstract class have Constructor?**

Yes, when we define a class to be an Abstract Class it cannot be instantiated but that does not mean an Abstract class cannot have a constructor. Each abstract class must have a concrete subclass which will implement the abstract methods of that abstract class. Hence we can have a constructor in abstract classes.

**Can there be any abstract method without abstract class?**

Yes, interface can have abstract method.

**Why can't we instantiate an abstract class?**

It's because abstract class doesn't have the full implementation of its methods.

**Do we need to import java.lang package?**

No. It is imported by default.

**What is JIT compiler?**

JIT, stands for Just In Time, compiler compiles the bytecodes of a method into native machine code, compiling it 'just in time' to run.

**What is JRE?**

**JRE:** Java Runtime Environment.

**What is platform?**

It is a combination of hardware and system software that will mostly run all the same software.

**What is OOP stands for? Write all the OOP features.**

**OOP:** Object Oriented Programming.

**Features:**

-   Abstraction
-   Encapsulation
-   Inheritance
-   Polymorphism

**What is the difference between encapsulation and abstraction?**

Encapsulation is wrapping, just hiding properties and methods. Encapsulation is used for hiding the code and data in a single unit to protect the data from the outside the world. A class is the best example of encapsulation.

Abstraction, on the other hand, means showing only the necessary details to the intended user.

**What is Inheritance? What are the types of Inheritance?**

It is a mechanism where a new class is derived from an existing class with all the properties and methods.

There are three types of inheritance in java: single, multilevel and hierarchical.

**Write down and explain different types of Inheritance.**

-   **Single:** only one subclass is derived from the superclass.
-   **Multilevel:** there is a subclass of a superclass and this subclass is a superclass of another subclass.
-   **Hierarchical:** when a superclass has multiple subclasses.

**Does java support multiple Inheritance?**

No. One class can inherit only from another class.

**How do you restrict a member of a class from inheriting to its subclasses?**

By declaring the class as final or by declaring all members of the class private.

**You know that all classes in java are inherited from java.lang.Object class. Are interfaces also inherited from Object class?**

Any class implementing any interface is also derived from Object class.

**Which class is the superclass for every class ?**

Object class.

**What is Polymorphism?**

It describes a language's ability to process objects of various types and classes through a single, uniform interface.

**What are the different types of Polymorphism and when that happen.**

There are two types of polymorphism in Java:

-   **Static Polymorphism:** also known as compile time polymorphism.
-   **Dynamic Polymorphism:** also is known as runtime polymorphism.

**What is Java API?**

Java application programming interface (API) is a list of all classes that are part of the Java development kit (JDK).

**What is the use of 'super' keyword in java? Explain in every level.**

Super is used to call the constructor, methods and properties of parent class. We can also use the super keyword in the sub class when we want to invoke a method from the parent class which is overridden in the subclass.

**Can we override private methods in Java?**

No, a private method cannot be overridden since it is not visible from any other class.

**What is static variable and static method in java?**

**Static variable** is also known as class variable, can be accessed directly by the class name and doesn't need any object. If one object changes a static variable value, it changes for all other objects.

**Static method** is a method which belongs to the class and not to the object (instance). It can be accessed directly by the class name and doesn't need any object.

**What is the difference between a final variable and a static variable?**

Final variable means the value can't be changed. Without final, any object can change the value of the variable.

Static variable means there is only one copy of the variable in memory shared by all instances of the class.

**What is final, finally and finalize?**

-   **Final** class can't be inherited, final method can't be overridden and final variable value can't be changed.
-   **Finally** is used to place important code, it will be executed whether the exception is handled or not.
-   **Finalize** is used to perform clean up processing just before the object is garbage collected.

**When finally block is executed in java?**

The finally block is placed after a 'try and catch' block. The finally block contains code that will be executed whether or not an exception is thrown in the try block.

**What is an Exception?**

An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.

**What is the difference between error and exception in java?**

An error indicates serious problems that a reasonable application should not try to catch.

An exception indicates conditions that a reasonable application might want to catch.

**How are the Exceptions handled in java?**

If a method does not handle a checked exception, the method must declare it using the throws keyword. The throws keyword appears at the end of a method's signature. We can throw an exception, either a newly instantiated one or an exception that you just caught, by using the throw keyword.

**What is nested class?**

It means that a class can be declared inside another class.

**What is the use of FileReader and BufferedReader class?**

-   **FileReader** class is a general tool to read in characters from a File.
-   **BufferedReader** class can wrap around Readers, like FileReader, to buffer the input and improve efficiency.

**Write few IntelliJ shortcuts.**

```
psvm 		- public static void main
sout 		- System.out.println
ctrl + space 	- basic code completion
cmd + / 	- single line comment
Opt + cmd + / 	- block comment
cmd + S 	- save all the changes
ctrl + R 	- run the program
```

**What is Git and GitHub?**

-   **Git** is the distributed version control system. It is responsible for keeping track of changes to content (usually source code files), and it provides mechanisms for sharing that content with others.
-   **GitHub** is a company that provides Git repository hosting.

**Type 10 git commands with definition.**

```
git init 			- create a new local repo
git add <filename> 		- add file to staging
git add * 			- add files to staging
git commit -m "message"		- commit any changes
git push origin master 		- send changes to remote repo
git status 			- see what files are changed
git remote add origin <server> 	- add remote repo to the local
git remote -v 			- list all remote repos
git push origin <branchname> 	- push local to the remote branch
git pull 			- fetch and merge changes
```

**What is Enum in java?**

Enum is used to represent a group of named constants in Java.

**What is Singleton class?**

Singleton class is a class that can have only one object at a time.

**Which classes are candidates of Singleton? Which kind of class do you make Singleton in Java?**

Any class which will be available to the whole application and will have only one instance. Runtime class is one example of singleton.

**What is array in java?**

Array is a data structure. It is a container object that holds a fixed number of values of a single type.

**Declare an Integer array to store 10 values into it and use Scanner class to take user input and then retrieve those values.**

```
Scanner input = new Scanner(System.in);
Integer[] numbers = new Integer[10];

// take user input
for (int i = 0; i < numbers.length; i++)
{
    System.out.println("Please enter a number: ");
    numbers[i] = input.nextInt();
}

// retrieve values
System.out.println(Arrays.toString(numbers));
```

**Write a java code to convert String to Integer and Integer to String.**

```
String s = "2020";
int i = Integer.parseInt(s);
System.out.println(i);          //Output : 2020

int i = 2020;
String s = Integer.toString(i);
System.out.println(s);          //Output : 2020
```

**Write String vs StringBuffer vs StringBuilder.**

String is immutable, if we try to alter their values, another object gets created, whereas StringBuffer and StringBuilder are mutable so they can change their values.

**What is the use of loop? Write all different kind of loop.**

Loop is used for repetition of a set of instructions/functions.

There are three loops which are used mostly: do-while, while and for loop.

**What is the difference between "while" loop and "do-while" loop?**

-   **while loop** checks the condition first, then goes to the statements block.
-   **do-while loop** goes to the statements block first, then checks the condition.

**What is the Collection API?**

The Collection API is a set of classes and interfaces that support operation on collections of objects. These classes and interfaces are more flexible, more powerful, and more regular than the vectors, arrays, and hashtables if effectively replaces.

Example of classes:

-   HashSet
-   HashMap
-   ArrayList
-   LinkedList
-   TreeSet
-   TreeMap

Example of interfaces:

-   Collection
-   Set
-   List
-   Map

**What is LinkedList in java?**

Java LinkedList class uses doubly linked list to store the elements. It provides a linked-list data structure.

**What is Stack in java?**

Stack is a subclass of Vector that implements a standard last-in, first-out stack.

**What is Queue in java?**

Queue is a subtype of java.util.Collection interface. It is an ordered list of objects with its use limited to inserting elements at the end of list and deleting elements from the start of list i.e. it follows FIFO principle.

**what is the difference between a stack and a queue?**

Stack is a collection of objects that works in LIFO (Last in First out) mechanism while Queue is FIFO (First in First out). This means that the object that is inserted first is removed last in a stack while an object that is inserted first is removed first in a queue.

**What is Map in java?**

The Map interface maps unique keys to values. A key is an object that we use to retrieve a value at a later date.

**What is the difference between HashSet, HashMap and Hashtable?**

**Hashtable**

Hashtable is basically a data structure to retain values of key-value pair.

-   It does not allow null for both key and value. It will throw NullPointerException.
-   Hashtable does not maintain insertion order. The order is defined by the Hash function. So only use this if you do not need data in order.
-   It is synchronized. It is slow. Only one thread can access in one time.

**HashMap**

Like Hashtable it also accepts key value pair.

-   It allows null for both key and value.
-   HashMap does not maintain insertion order. The order is defined by the Hash function.
-   It is not synchronized. It will have better performance.

**HashSet**

HashSet does not allow duplicate values.

-   It provides add method rather put method.
-   You also use its contain method to check whether the object is already available in HashSet.
-   HashSet can be used where you want to maintain a unique list.

**What is Tree in java?**

A Tree is a non-linear data structure where data objects are organized in terms of hierarchical relationship.

**What is Graph in java?**

Graph is a data structure that consists of following two components:

1.  A finite set of vertices also called as nodes.
2.  A finite set of ordered pair of the form (u, v) called as edge.

**What is Iterator in java?**

Iterators are used in Collection framework in Java to retrieve elements one by one.
