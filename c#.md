C# critera

* Language purpose/genisis
  * C# was created to enable developers to build applications on the .NET framework and the syntax as well as functionality is very similar to java. This language was developed to make it easier to build apps on the .NET framework. By building these applcations on the .NET framework developers can call the code (in the framework) without writing it, and thus reducing the time it takes to build one of these apps.
* Unique features of the language
  * The .NET framework is not only expansive but is periodically updated at a faster rate than Java. This allows c# to shine through as the more up to date candidate. This also alows developers to build with the newest tools and technologies.
* Name spaces (example code needed)
  * C# uses namespaces heavily in two different ways. 
    * The .NET framework uses namespaces to organize its classes.
    * The traditional, declaring your own namespaces to control the scope of the class (method and variables).
  * In c# we use the 'using' keyword which helps save the developer time that would be wasted on specifying the full name every time a method inside the class is to be called. For example " using Namespace; "
  * In many cases using an 'alias' for a namespace is useful. If you have a namespace that has nested namespaces, it would be good practice to use an 'alias'. for example " using alias = Project.Service.Nested; "
* Types
    * bool, char, byte sbyte, uint, long, ulong, object, ushort. string. With Object and String as the only non-simple types.
    * Are both reference and value types supported? http://www.albahari.com/valuevsreftypes.aspx
    * In C# both reference and value types are supported. C# provides two types - a class and a struct. Structs can have similar members as classes, which can be fields, methods, perperties, or operators.
    * Reference types are created on the heap. The following types are Reference types: dynamic, object, string. In order to declare a reference type you must use one of the following keywords: class, interface, delegate.
    * Value types are created on the stack. The following types are value types: structs and enumerations.
      * Structs fall into the following categories: Numeric types (integra, floating-point, and decimal types), bool, and user defined structs.
    * It is possible to create a new value type in C#. C# does not however, have a type system that supports checking integer ranges at compile time, so you would not be able to change the range of your new type with a range from 1-100 when the limit is set to 0-255.
* Classes
  * Defining https://docs.microsoft.com/en-us/dotnet/articles/csharp/programming-guide/classes-and-structs/classes
  * A class in C# is essentially a data structure that encapsulates a set of data and behaviors that belong together as a logical unit, and is used similarly to java, as a bluepring used to create instances or objects at run time. To define a class, you must define the access level, followed by the 'class' keyword and the name of your class. What follows are nay fields (controls the state) and methods(controls the behavior).
  * Creating new instances https://docs.microsoft.com/en-us/dotnet/articles/csharp/programming-guide/classes-and-structs/instance-constructors
  * In C# Constructors are the primary way of creating a new instance as well as initilizing them at run time.
  * Destructing/de-initializing https://docs.microsoft.com/en-us/dotnet/articles/csharp/programming-guide/classes-and-structs/destructors
  * In C# you can only destruct classes, desructors cannot be defined in structs. Classes may only have one destructor, they cannot be inherited or overloaded, nor can they be called (they are called automaticly). A destructor may not take modifiers or have parameters.
* Instance reference name in data type (class)
  * In C# we use the 'this' keyword to refer to the current instance of the class.
--------------------------------------------------------------------------------------------------
* Procedural Programming
  * Both C# and Java support procedural programming, as it is up to the developer to implement the OOP features the language brings. Procedural programming consists of sequences of imperative statements, assignments, tests, loops and invocations of sub procedures. This type of programming is not encouraged in OOP due to the challenges and difficulties it brings with maintenance of the code-base in large-scale projects.

* Functional Programming
  * C# can be considered a functional programming language as it does provide some features unique to higher order programming. As of C# 2.0, developers are allowed to pass and return functions as values for higher order functions, and includes limited support for anonymous delegates. Anonymous delegates allow the programmer to encapsulate a method reference in a *delegate* object. Delegate's do not care about the class of the object it references, only the method's argument types and return types must match. In C# 3.0 and 3.5 also came improved support for anonymous functions as true closures.

* MultiThreading
    * C# supports parallel execution of applications through multithreading, like many other languages. This functionality is dependent on the *System.Threading.Thread* class, which enables creation and access of threads adjacent to the main thread. This system *Thread* class has a *CurrentThread* property that is used to access threads. Similar to other languages, there are four distinct states threads can be in. Unstarted, Ready, Not Runnable, and Dead. When a thread has been created, but not yet started execution it lies in the Unstarted state. Once the *start()* method of the Thread is called, it enters the *Ready* state. This signifies the thread is waiting to be scheduled on the CPU. If thread is interrupted by the *sleep()* method, the *wait()* method, or I/O operations, it is placed in the *Not Runnable* state until it can be scheduled on the CPU again. Lastly, when a thread completes execution or is aborted, it is placed in the *Dead* state. C# also supports thread priority levels, but it's important not to set priorities of user threads too high. If this is done it is possible to lock up the host platform due to placing user tasks above system ones.
