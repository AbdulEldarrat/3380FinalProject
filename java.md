Java Critera

* Language purpose/genisis
  * Java was created to address the issue of uniformality. The creators of java wanted to have a language tat would be as few implemnetation dependencies as possible. Meant to "write once and run anywhere". Java wasn't necessaritly meant to replace any other languag but was somewhat derived from c and c++ but more high level language then the both of them.
* Unique features of the language
  * A Java Application can run on any operating system that can run a JVM (Java Virtual Machine). This makes Java a language that nearly anyone can compile and run on their machine.
* Name spaces (https://www.cs.ait.ac.th/~on/O/oreilly/java-ent/jnut/ch02_11.htm)
  * In java, the platform includes packages that start with java, org.omg., javax, along with other that are defined in Sun's standard extensions. Packages can hold subPackages which holds classes. Packages may also hold classes directly without any subpackages.
  * To specify a class is to be part of a package you must use the 'package' keyword before defining the package.subPackage.subSubPackageWhereTheFileIs;
  * packages are used to to "partition the java namespace and prevent name collisions" or in other words be able to reuse names for classes while the compiler is still able to discern the difference between the two.
* Types
    * Java supports a multitude of types from Primitive data types: byte, short, int, long, float, double, boolean, and char. Java also has Reference data types, which would be any variable that is created using defined constructors of its class. The refeence variables are used to do just that, reference. The default value of any reference variable is null. In java you also have objects and classes. A class is used as a blueprint of the object with the fields storing the state and the method defining the behavior of the object. You cannot create a new primitive data type, you can  however mock a new object to act as if it was though.
  
 
-------------------------------------------------------------
* MultiThreading
  * Like C#, Java also has defined states for threads. The *New* state is for threads that have not yet started execution. Once the *start()* method of the thread has been called, it moves to the *Runnable* state. In this state the thread is executing within the JVM. If a thread attempts to access a resource and it is blocked from waiting for that resource lock, it is placed in the *Blocked* state. If a thread is waiting indefinitely for another thread to perform an action, it moves to the *Waiting* state. Threads can be given timed waits, and if they are waiting on another thread for a specified amount of time they move to the *Timed Waiting* state. Lastly is the *Terminated* state, reserved for threads that have exited execution. Threads can be created by extending an existing **Thread** class, or implementing the **Runnable** interface. However the thread is created, it must begin execution using the *start()* method. Java threads can also be given priority to determine which threads should be scheduled before others, but how this is interpreted is up to the host platform and does not guarantee thread execution order.
