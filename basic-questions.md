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

<details>
  <summary>10. What is classloader?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Classloader is a subsystem of JVM (Java Virtual Machine) used to load class files. When a Java program is executed, it is first loaded by the classloader. There are three built-in classloaders in Java:

**1. Bootstrap ClassLoader:**

- This is the first classloader and serves as the superclass of the Extension classloader.
- It loads the `rt.jar` file, which contains class files for Java Standard Edition, including classes from packages such as `java.lang`, `java.net`, `java.util`, `java.io`, `java.sql`, and more.

**2. Extension ClassLoader:**

- A child classloader of the Bootstrap ClassLoader and the parent classloader of the System ClassLoader.
- It loads JAR files located inside the `$JAVA_HOME/jre/lib/ext` directory.

**3. System/Application ClassLoader:**

- A child classloader of the Extension ClassLoader.
- It loads class files from the classpath. By default, the classpath is set to the current directory.
- Also known as the Application ClassLoader.

Each classloader has a specific role in loading classes, and they form a hierarchy to efficiently manage class loading in Java.</p>

</details>
<details>
  <summary>11. What are keywords in Java?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Keywords in Java are reserved words that have predefined meanings and cannot be used as identifiers (variable names, class names, etc.). They are an integral part of the Java programming language and serve specific purposes in defining the structure and behavior of a Java program. Some common Java keywords include:

- **abstract**
- **assert**
- **boolean**
- **break**
- **byte**
- **case**
- **catch**
- **char**
- **class**
- **const**
- **continue**
- **default**
- **do**
- **double**
- **else**
- **enum**
- **extends**
- **final**
- **finally**
- **float**
- **for**
- **if**
- **implements**
- **import**
- **instanceof**
- **int**
- **interface**
- **long**
- **native**
- **new**
- **package**
- **private**
- **protected**
- **public**
- **return**
- **short**
- **static**
- **strictfp**
- **super**
- **switch**
- **synchronized**
- **this**
- **throw**
- **throws**
- **transient**
- **try**
- **void**
- **volatile**
- **while**

These keywords play crucial roles in defining classes, methods, control flow, data types, and other aspects of Java programming.</p>

</details>

<details>
  <summary>12. What is ENUM in Java?</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In Java, an ENUM (enumeration) is a special data type that consists of a fixed set of constant values. It provides a way to create a group of related named constants, making the code more readable and maintainable. Enums were introduced in Java 5 to address the need for a type-safe way to represent a set of predefined values.

Key characteristics of ENUMs in Java:

- **Declaration:** Enums are declared using the `enum` keyword.

- **Instance Creation:** Enum constants are created implicitly and are static and final. For example, if you declare an enum named `Color`, its constants (e.g., RED, GREEN, BLUE) are automatically created.

- **Methods:** Enums can have methods, fields, and constructors. Each constant in the enum is an instance of the enum type.

- **Iteration:** Enums can be iterated using the enhanced for loop, and the order of constants is the order in which they are declared.

Example of a simple ENUM in Java:

```java
    enum Day {
        SUNDAY, MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY
    }
```
</details>
<details>
  <summary>13. Memory Management in Java ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Java employs automatic memory management through garbage collection. In this approach, the Java Virtual Machine (JVM) automatically deallocates memory occupied by objects that are no longer reachable. Developers are relieved from direct control over memory allocation, minimizing the risk of memory leaks and simplifying memory management.</p>
</details>

<details>
  <summary>14. JVM vs. HotSpot Technologies ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">The Java Virtual Machine (JVM) is an abstract machine providing a runtime environment for Java bytecode execution. HotSpot, developed by Oracle, is a specific implementation of the JVM. It includes features like an adaptive compiler and garbage collector, focusing on high performance. HotSpot dynamically recompiles bytecode into native machine code, optimizing runtime performance compared to a generic JVM.</p>
</details>

<details>
  <summary>15. Multithreading and its Significance ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Multithreading is a concurrent execution mechanism where multiple threads exist within the context of a single process. Threads are independent paths of execution, allowing programs to perform multiple tasks concurrently. This concurrency enhances system utilization, responsiveness, and can lead to more efficient program execution, especially in tasks with parallelizable components.</p>
</details>

<details>
  <summary>16. diffrentiate Threads vs. Processes ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Threads and processes are both units of execution, but they differ in their memory space. Threads within the same process share the same memory space, while processes have separate memory spaces. Threads are lighter-weight than processes and can communicate more easily. However, processes provide stronger isolation, making them more robust in certain scenarios.</p>
</details>

<details>
  <summary>17. Thread Class and its Methods ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In Java, the `Thread` class is part of the `java.lang` package and provides methods to create and control threads. Some essential methods include `start()` to initiate the thread's execution, `run()` where the thread's logic is defined, `sleep(long millis)` for pausing a thread's execution, and `join()` for waiting until a thread completes its execution.</p>
</details>

<details>
  <summary>18. Creating and Starting a Thread in Java ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">To create and start a thread in Java, one can extend the `Thread` class or implement the `Runnable` interface. Extending `Thread` involves overriding the `run()` method with the thread's logic. Alternatively, implementing `Runnable` requires defining the `run()` method in a separate class. After creating an instance, the `start()` method is invoked to begin the thread's execution.</p>
</details>

<details>
  <summary>19. Synchronized Keyword and its Usage ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In Java, the `synchronized` keyword is used to control access to critical sections of code. When a method or a block of code is marked as synchronized, only one thread can execute it at a time. This prevents data corruption in scenarios where multiple threads might access shared resources simultaneously. The synchronization ensures data consistency and avoids race conditions.</p>
</details>
<details>
  <summary>20. Best Practices for Writing Clean and Efficient Java Code ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">To write clean and efficient Java code, it's crucial to follow coding standards, use descriptive naming, choose appropriate data structures, minimize unnecessary object creation, optimize loops, handle exceptions judiciously, control concurrency, and conduct regular code reviews. These practices contribute to readable, maintainable, and high-performance Java code.</p>
</details>


<details>
  <summary>21. Reading and Writing Data from/to Files in Java ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In Java, reading and writing data from/to files is commonly achieved using classes from the `java.io` package. To read data, you can use classes like `FileReader` along with `BufferedReader` for efficient reading. For writing, `FileWriter` and `BufferedWriter` are commonly used. The `java.nio.file` package also provides more advanced file operations through the `Files` class.</p>
</details>

<details>
  <summary>22. Handling User Input and Output in Java ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">User input and output in Java can be managed using the `Scanner` class for input and `System.out.println()` or `System.out.print()` for output. The `Scanner` class allows reading various types of input, such as integers, doubles, and strings, from the console. For output, the `System.out.println()` method prints data to the console, while `System.out.print()` prints without a newline character.</p>
</details>

<details>
  <summary>23. Scanner Class and its Methods with Examples ?</summary>

  <p style="background-color: #f2f2f2; margin-left: 20px;">
  Here's an example demonstrating the usage of the `Scanner` class for user input in Java:
  </p>

  ```java
  import java.util.Scanner;

  public class UserInputExample {
      public static void main(String[] args) {
          // Create a Scanner object to read input
          Scanner scanner = new Scanner(System.in);

          // Prompt the user for input
          System.out.print("Enter your name: ");

          // Read a line of text
          String name = scanner.nextLine();

          // Prompt for an integer
          System.out.print("Enter your age: ");
          int age = scanner.nextInt();

          // Display the input
          System.out.println("Hello, " + name + "! You are " + age + " years old.");

          // Close the scanner to prevent resource leak
          scanner.close();
      }
  }
  ```

  In this example, the `Scanner` class is used to read the user's name as a string and age as an integer from the console.
  </p>
</details>

<details>
  <summary>24. Collections Framework in Java ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">The Collections Framework in Java is a set of interfaces and classes that provide a way to organize and manipulate groups of objects. It is designed to be flexible, high-performance, and interoperable. The framework includes several core interfaces such as `Collection`, `List`, `Set`, `Map`, and their respective implementations.</p>
</details>

<details>
  <summary>25. List Interface ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">The `List` interface extends the `Collection` interface and represents an ordered collection of elements where duplicates are allowed. Some common implementations of the `List` interface are `ArrayList`, `LinkedList`, and `Vector`.</p>
</details>

<details>
  <summary>26. Set Interface ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">The `Set` interface extends the `Collection` interface and represents a collection of unique elements. It does not allow duplicate elements. Common implementations include `HashSet`, `LinkedHashSet`, and `TreeSet`.</p>
</details>

<details>
  <summary>27. Map Interface ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">The `Map` interface represents a collection of key-value pairs, where each key is associated with exactly one value. It does not extend the `Collection` interface. Common implementations include `HashMap`, `LinkedHashMap`, and `TreeMap`.</p>
</details>

<details>
  <summary>28. Example Usage of List, Set, and Map ?</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">
  
  ```java
  import java.util.ArrayList;
  import java.util.HashSet;
  import java.util.HashMap;
  import java.util.List;
  import java.util.Set;
  import java.util.Map;

  public class CollectionsExample {
      public static void main(String[] args) {
          // List Example
          List<String> list = new ArrayList<>();
          list.add("Java");
          list.add("Python");
          list.add("C++");
          System.out.println("List: " + list);

          // Set Example
          Set<Integer> set = new HashSet<>();
          set.add(10);
          set.add(20);
          set.add(30);
          set.add(20); // Duplicate, not allowed in a Set
          System.out.println("Set: " + set);

          // Map Example
          Map<String, Integer> map = new HashMap<>();
          map.put("One", 1);
          map.put("Two", 2);
          map.put("Three", 3);
          System.out.println("Map: " + map);
      }
  }
  ```
  
  This example demonstrates the usage of `List`, `Set`, and `Map`. The `List` contains strings, the `Set` contains integers (with duplicates not allowed), and the `Map` associates string keys with integer values.
  </p>
</details>

<details>
  <summary>29. Difference between Stacks, Queues, and Linked Lists:</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Stacks, queues, and linked lists are fundamental data structures, each serving specific purposes.</p>
  - **Stack:** Follows Last In, First Out (LIFO) order. Elements are added and removed from the same end, known as the "top" of the stack.
  - **Queue:** Follows First In, First Out (FIFO) order. Elements are added at the rear (enqueue) and removed from the front (dequeue) of the queue.
  - **Linked List:** A collection of nodes, each containing data and a reference to the next node. It can be singly or doubly linked.
</details>

<details>
  <summary>30. Simple Stack and Queue Implementation in Java:</summary>

  <details>
    <summary>**Stack Implementation:**</summary>

  ```java
  public class Stack {
      private int maxSize;
      private int[] stackArray;
      private int top;

      public Stack(int size) {
          maxSize = size;
          stackArray = new int[maxSize];
          top = -1;
      }

      public void push(int value) {
          if (top < maxSize - 1) {
              stackArray[++top] = value;
          } else {
              System.out.println("Stack is full. Cannot push " + value);
          }
      }

      public int pop() {
          if (top >= 0) {
              return stackArray[top--];
          } else {
              System.out.println("Stack is empty.");
              return -1;
          }
      }

      public int peek() {
          if (top >= 0) {
              return stackArray[top];
          } else {
              System.out.println("Stack is empty.");
              return -1;
          }
      }

      public boolean isEmpty() {
          return top == -1;
      }

      public boolean isFull() {
          return top == maxSize - 1;
      }
  }
  ```

  </details>

  <details>
    <summary>**Queue Implementation:**</summary>

  ```java
  public class Queue {
      private int maxSize;
      private int[] queueArray;
      private int front;
      private int rear;

      public Queue(int size) {
          maxSize = size;
          queueArray = new int[maxSize];
          front = 0;
          rear = -1;
      }

      public void enqueue(int value) {
          if (rear < maxSize - 1) {
              queueArray[++rear] = value;
          } else {
              System.out.println("Queue is full. Cannot enqueue " + value);
          }
      }

      public int dequeue() {
          if (!isEmpty()) {
              int removedValue = queueArray[front++];
              if (front > rear) {
                  front = 0;
                  rear = -1;
              }
              return removedValue;
          } else {
              System.out.println("Queue is empty.");
              return -1;
          }
      }

      public int peek() {
          if (!isEmpty()) {
              return queueArray[front];
          } else {
              System.out.println("Queue is empty.");
              return -1;
          }
      }

      public boolean isEmpty() {
          return rear == -1 || front > rear;
      }

      public boolean isFull() {
          return rear == maxSize - 1;
      }
  }
  ```

  </details>

</details>

<details>
  <summary>31. Big O Notation and its Importance:</summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Big O notation is a mathematical notation that describes the performance or complexity of an algorithm. It provides an upper bound on the growth rate of the algorithm in the worst-case scenario. The notation is crucial in algorithm analysis for the following reasons:</p>
  - **Quantifying Efficiency:** Big O notation allows us to express the efficiency of algorithms in a standardized way, making it easier to compare and analyze different algorithms.
  - **Identifying Dominant Operations:** It helps in identifying the operations that dominate the overall runtime as the input size grows, focusing on the most significant factors.
  - **Scaling Predictions:** Big O provides insights into how the algorithm's performance scales with the input size, helping predict how the algorithm will perform as the problem size increases.
  - **Optimization Guidance:** It guides optimization efforts by highlighting areas of the algorithm that have the most impact on performance.
</details>


<details>
  <summary>32. Difference between final and finalize:</summary>

  | Feature           | final                                    | finalize                              |
  |-------------------|------------------------------------------|---------------------------------------|
  | Usage             | Used with variables, methods, and classes to make them unmodifiable, unextendable, or unchanged. | A method in the Object class that is called by the garbage collector before an object is garbage collected. |
  | Scope             | Applicable to variables, methods, and classes. | Specifically related to garbage collection in Java and is part of the Object class. |
  | Purpose           | Provides immutability, prevents method overriding, and restricts class extension. | Intended for cleanup operations before an object is reclaimed by the garbage collector. |
  | Inheritance       | Can be used in class declarations to prevent further subclassing. | Not directly related to inheritance. |
  | Keyword Usage     | `final` keyword is used.                     | `finalize()` method is used.            |

</details>
<details>
  <summary>33. Explain pass by value and pass by reference in Java.</summary>

In Java, when passing arguments to methods, the terms "pass by value" and "pass by reference" are often used to describe how the values are transferred.

1. **Pass by Value:**
   - Java is strictly "pass by value." This means that when you pass a primitive data type (like `int`, `float`, etc.) to a method, you are passing a copy of the actual value.
   - Modifications to the parameter inside the method do not affect the original value outside the method.

   ```java
   public class PassByValueExample {
       public static void main(String[] args) {
           int number = 5;
           modifyValue(number);
           System.out.println("Original value: " + number);
       }

       static void modifyValue(int num) {
           num = num * 2;
           System.out.println("Modified value: " + num);
       }
   }
   ```

   In this example, the modification inside the `modifyValue` method does not affect the original `number` outside the method.

2. **Pass by Reference (not applicable in Java):**
   - In some programming languages, "pass by reference" means passing a reference (memory address) to the original variable. Changes made to the parameter inside the method reflect in the original variable.
   - Java, however, does not support true pass by reference for objects. When you pass an object to a method, you are passing the reference to the object by value.

   ```java
   public class PassByReferenceExample {
       public static void main(String[] args) {
           StringBuilder text = new StringBuilder("Hello");
           modifyText(text);
           System.out.println("Original text: " + text);
       }

       static void modifyText(StringBuilder str) {
           str.append(", World!");
           System.out.println("Modified text: " + str);
       }
   }
   ```

   In this example, the modifications inside the `modifyText` method affect the original `text` outside the method. However, it's crucial to understand that the reference itself is passed by value, not the object.
</details>
<details>
  <summary>34. Explain wrapper classes in Java.</summary>

Wrapper classes in Java serve as a mechanism to convert primitive data types into objects. They "wrap" primitive data types in an object so that they can be included in activities reserved for objects, like being added to collections. The Java programming language provides a set of wrapper classes for each primitive data type.

**Example:**

```java
// Primitive data type
int primitiveInt = 42;

// Wrapper class for int
Integer wrappedInt = Integer.valueOf(primitiveInt);

// Performing operations with the wrapper class
int result = wrappedInt + 10;

// Converting back to primitive data type
int unwrappedInt = wrappedInt.intValue();
```

In the example above, `Integer` is the wrapper class for the `int` primitive data type. It allows the primitive `int` to be used in contexts where objects are required. The process of converting a primitive type to its corresponding wrapper class is called autoboxing, and the reverse process is called unboxing.

Wrapper classes also provide utility methods for various operations, making it convenient to work with primitive types in an object-oriented manner. Common wrapper classes include `Integer`, `Double`, `Boolean`, etc., each corresponding to a specific primitive type.
</details>
<details>
  <summary>35. Explain constructor overloading in Java.</summary>

Constructor overloading in Java refers to the concept of defining multiple constructors within a class, each having a different set of parameters. This allows a class to provide multiple ways to instantiate objects, accommodating various initialization scenarios.

**Example:**

```java
public class MyClass {
    int value;

    // Constructor with no parameters
    public MyClass() {
        value = 0;
    }

    // Constructor with a single parameter
    public MyClass(int initialValue) {
        value = initialValue;
    }

    // Constructor with two parameters
    public MyClass(int initialValue, boolean doubleValue) {
        value = doubleValue ? 2 * initialValue : initialValue;
    }
}

// Instantiating objects using different constructors
MyClass obj1 = new MyClass();              // Initializes with default value
MyClass obj2 = new MyClass(10);            // Initializes with specified value
MyClass obj3 = new MyClass(5, true);       // Initializes with doubled value
```

In the example above, the `MyClass` class has three constructors, each catering to different initialization requirements. The appropriate constructor is chosen based on the number and types of arguments provided during object instantiation. This flexibility enhances the usability and versatility of the class.
</details>
<details>
  <summary>36. Garbage Collection in Java:</summary>

  <p style="background-color: #f2f2f2; margin-left: 20px;">Garbage collection in Java is the automatic process of identifying and reclaiming the memory occupied by objects that are no longer reachable or in use by the program. Java employs an automatic garbage collector to handle memory management, relieving developers from manually deallocating memory.</p>

  <p style="background-color: #f2f2f2; margin-left: 20px;"><strong>Functions in Garbage Collection:</strong></p>

  <ol style="background-color: #f2f2f2; margin-left: 40px;">
    <li><strong>Identification of Unreachable Objects:</strong> The garbage collector identifies objects that are no longer reachable from the root of the object graph, typically starting from the main method.</li>
    <li><strong>Reclamation of Memory:</strong> Once unreachable objects are identified, the garbage collector reclaims the memory occupied by these objects, making it available for new allocations.</li>
    <li><strong>Compactification (Optional):</strong> Some garbage collectors perform compactification, where the remaining objects are moved to a contiguous block of memory, reducing memory fragmentation.</li>
  </ol>

  <p style="background-color: #f2f2f2; margin-left: 20px;"><strong>Java Garbage Collection Process:</strong></p>

  <p style="background-color: #f2f2f2; margin-left: 40px;">Java uses a generational garbage collection algorithm, primarily dividing the heap into two main areas: the Young Generation and the Old Generation.</p>

  <ol style="background-color: #f2f2f2; margin-left: 40px;">
    <li><strong>Young Generation:</strong> Newly created objects are initially allocated in the Young Generation. A Minor Garbage Collection is performed frequently in this area.</li>
    <li><strong>Old Generation:</strong> Objects that survive multiple Minor Garbage Collections are eventually moved to the Old Generation. Major Garbage Collection is less frequent but involves the entire heap.</li>
    <li><strong>Garbage Collector Types:</strong> Java has various garbage collector implementations, such as Serial, Parallel, CMS (Concurrent Mark-Sweep), G1 (Garbage First), each suited for different scenarios and performance requirements.</li>
  </ol>

  <p style="background-color: #f2f2f2; margin-left: 20px;">In summary, Java's garbage collection automates memory management by identifying and reclaiming memory occupied by unreachable objects, ensuring efficient and reliable memory usage in Java applications.</p>
</details>

<details>
  <summary>37. Difference between `static` and `final` Keywords:</summary>

  <table style="background-color: #f2f2f2; margin-left: 20px; border-collapse: collapse; width: 80%;">
    <tr>
      <th style="border: 1px solid #dddddd; text-align: left; padding: 8px;">Feature</th>
      <th style="border: 1px solid #dddddd; text-align: left; padding: 8px;">`static` Keyword</th>
      <th style="border: 1px solid #dddddd; text-align: left; padding: 8px;">`final` Keyword</th>
    </tr>
    <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">Scope</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Belongs to the class and shared among all instances of the class.</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Indicates that a variable, method, or class cannot be changed or overridden.</td>
    </tr>
    <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">Usage (Variable)</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Used to create class-level variables or methods that are shared among all instances.</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Used to create constants (immutable variables) that cannot be modified after initialization.</td>
    </tr>
    <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">Usage (Method)</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Used to create class-level methods that can be called without creating an instance of the class.</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Used to indicate that a method cannot be overridden by subclasses.</td>
    </tr>
    <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">Memory Allocation</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Memory is allocated once for the `static` variable or method in the class area.</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Memory is allocated when the `final` variable is initialized, and it cannot be changed afterwards.</td>
    </tr>
    <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">Inheritance</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">`static` members can be inherited, and changes to them in a subclass affect the superclass.</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">`final` members cannot be overridden in subclasses, preserving their functionality.</td>
    </tr>
  </table>

  <p style="background-color: #f2f2f2; margin-left: 20px;">In summary, the `static` keyword is used for creating class-level variables and methods that are shared among all instances, while the `final` keyword is used for indicating immutability, making variables, methods, or classes unchangeable or unextendable.</p>
</details>

If you have more questions or need further clarification, feel free to ask!