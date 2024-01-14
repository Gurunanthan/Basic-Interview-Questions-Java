<details>
  <summary>1. What is Java?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Java is a versatile, high-level, object-oriented programming language known for its platform independence and portability. Developed by Sun Microsystems (now owned by Oracle), Java is designed to be simple, secure, and robust. It follows the "Write Once, Run Anywhere" (WORA) principle, allowing Java programs to run on any device with a Java Virtual Machine (JVM). Java supports multithreading, which enables concurrent execution of tasks, making it suitable for building scalable and responsive applications. Its rich standard library and extensive ecosystem of third-party libraries contribute to its popularity in various domains, including web development, mobile app development, enterprise solutions, and more.</p>
</details>

<details>
  <summary>2. Why is Java not a pure object-oriented language?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Java is not considered a pure object-oriented language due to several factors. One reason is the inclusion of primitive data types (e.g., `int`, `float`, `char`) that are not treated as objects. Unlike in a pure object-oriented language, Java allows the use of these non-object types for efficiency and simplicity. Additionally, Java supports static members and methods, which are associated with the class itself rather than instances of the class. In a truly pure object-oriented language, all entities would be treated as objects, without the concept of static elements. Furthermore, Java's approach to inheritance differs from some pure object-oriented languages, as it supports interface-based multiple inheritance but not class-based multiple inheritance. Despite these deviations, Java remains predominantly object-oriented, emphasizing key OOP principles such as encapsulation, inheritance, and polymorphism in its design.</p>
</details>

<details>
  <summary>3. Difference between Heap and Stack Memory in Java and how Java utilizes them?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In Java, memory management involves two main areas: Heap and Stack.

**Heap Memory:**
Heap memory is primarily used for the dynamic allocation of objects during the runtime of a program. Objects created in the heap have a more extended lifespan and persist beyond the scope of the method or function that instantiated them. The heap is where the Java Virtual Machine (JVM) stores objects and their associated data. Garbage collection, a crucial aspect of Java memory management, automatically identifies and reclaims memory from objects that are no longer reachable or in use.

**Stack Memory:**
Stack memory, on the other hand, is employed for static memory allocation and holds local variables and references to objects within methods and blocks. Each thread in Java has its own stack, and the stack keeps track of the methods being called and their local variables. It operates on a Last-In-First-Out (LIFO) structure, where the last method called is the first one to be removed.</p>
</details>

<details>
  <summary>4. How Java Utilizes Heap and Stack?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Java utilizes the heap and stack memory areas for efficient memory management. Objects and their associated data are created and stored in the heap memory, enabling dynamic memory allocation during runtime. The stack memory, dedicated to method execution, manages local variables and method calls, ensuring a thread-specific execution environment. The separation of heap and stack memory allows Java to strike a balance between flexibility and efficiency, preventing memory leaks through automatic garbage collection in the heap and handling method calls in the stack.</p>
</details>

<details>
  <summary>5. How is Java different from C++?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Java and C++ differ in several key aspects. In terms of memory management, Java features automatic memory management with a garbage collector, while C++ provides developers with more control over memory but requires manual allocation and deallocation. Java is platform-independent, following the "Write Once, Run Anywhere" principle, compiling code into bytecode for execution on any device with a Java Virtual Machine (JVM). In contrast, C++ code needs separate compilation for each target platform, making it less portable.

In terms of language features, Java prioritizes simplicity and readability, lacking certain low-level features like pointers and explicit memory management found in C++. Java supports multiple inheritance through interfaces, whereas C++ supports both class-based and interface-based multiple inheritance, introducing flexibility but potentially leading to the "diamond problem."

Multithreading is integral to Java, with built-in support for creating and managing threads, while C++ also supports multithreading with variations between standards and implementations. Exception handling in Java is more structured, distinguishing between checked and unchecked exceptions, whereas C++ uses a combination of try, catch, and throw with a less rigid structure.

These differences highlight distinct design philosophies and use cases, with Java emphasizing simplicity, platform independence</p>
</details>
<details>
  <summary>6. What are the default values assigned to variables and instances in Java?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In Java, variables and instances are automatically assigned default values if they are not explicitly initialized. The default values depend on the data type:

**For Instance Variables (non-static fields):**

- Numeric types (byte, short, int, long, float, double): 0
- char: '\u0000' (null character)
- boolean: false
- Object references: null

**For Local Variables (method variables):**

- Local variables are automatically initialized with default values, and their scope is limited to the method or block in which they are declared. The default values for local variables are as follows:
  - Numeric types (byte, short, int, long, float, double): 0
  - char: '\u0000' (null character)
  - boolean: false
  - Object references: null

It's important to note that using local variables without initializing them can result in compilation errors, ensuring that developers explicitly assign values before using them in calculations or conditions.</p>
</details>


<details>
  <summary>7. How does the JIT compiler work in Java?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">The Just-In-Time (JIT) compiler is a key component of the Java Virtual Machine (JVM) responsible for enhancing the performance of Java programs. Initially, Java source code is compiled into bytecode by the Java compiler. During program execution in the JVM, the bytecode is interpreted, and the JIT compiler intervenes to translate frequently executed portions, known as "hotspots," into native machine code at runtime.

The JIT compiler employs profiling and monitoring techniques to identify hotspots by collecting data on method call frequencies and execution times. It selectively compiles only these hotspots, optimizing critical sections of the code dynamically. This selective compilation strategy enhances performance without spending unnecessary time on less frequently executed parts of the code.

The JIT compiler may employ caching to avoid redundant compilation of the same code during subsequent executions and perform in

lining, incorporating small and frequently called methods directly into the calling method to reduce method call overhead.

An important aspect of the JIT compiler is its adaptive nature. It continuously monitors the program's behavior during runtime, adapting its optimization strategies based on feedback. If the behavior of the program changes, the JIT compiler can recompile and optimize the code accordingly.

The JIT compiler's dynamic compilation and optimization contribute to the efficient execution of Java programs, providing a balance between platform independence and performance by generating native machine code tailored to the specific characteristics of the executing environment.</p>
</details>

<details>
  <summary style="cursor: pointer;">8. What are the features of the Java Programming language?</summary>
  <br>
  Java is a robust and versatile programming language known for several key features.

  - **Platform Independence:**
    Java code is designed to be platform-independent, allowing it to run on any device equipped with a Java Virtual Machine (JVM).

  - **Object-Oriented Paradigm:**
    Java follows the object-oriented programming (OOP) paradigm, emphasizing principles like encapsulation, inheritance, and polymorphism.

  - **Multithreading Support:**
    Java provides built-in support for multithreading, enabling the concurrent execution of multiple threads and enhancing program performance.

  - **Automatic Memory Management:**
    One of Java's strengths is its automatic garbage collection mechanism, which helps manage memory efficiently and reduces the risk of memory leaks.

  - **Rich Standard Library:**
    Java comes with a comprehensive standard library that includes a wide range of classes and methods, simplifying development tasks and extending functionality.

  - **Security Features:**
    Java incorporates robust security features, including a sandbox for applet security, making it a suitable choice for secure applications.

  - **Portability:**
    Following the "Write Once, Run Anywhere" (WORA) principle, Java allows code to be executed on various platforms without modification.

  - **Distributed Computing:**
    Java supports the creation of distributed applications through features like Remote Method Invocation (RMI), facilitating communication between distributed components.

  - **Dynamic Adaptability:**
    Java applications can dynamically adapt to changing environments, supporting features like dynamic loading of classes.
</details>


<details>
  <summary>9. How many types of memory areas are allocated by JVM?</summary>
  <br>
  Java Virtual Machine (JVM) allocates memory in various areas to manage the execution of Java programs. The main types of memory areas include:

  - **Class(Method) Area:**
    Class Area stores per-class structures such as the runtime constant pool, field, method data, and the code for methods.

  - **Heap:**
    Heap is the runtime data area where memory is allocated to objects created during program execution.

  - **Stack:**
    Java Stack stores frames, holding local variables and partial results. It plays a crucial role in method invocation and return. Each thread has a private JVM stack, created concurrently with the thread. A new frame is created for each method invocation, and a frame is destroyed when the method invocation completes.

  - **Program Counter Register:**
    The PC (program counter) register contains the address of the Java virtual machine instruction currently being executed.

  - **Native Method Stack:**
    Native Method Stack contains all the native methods used in the application.

</details>

