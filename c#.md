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
