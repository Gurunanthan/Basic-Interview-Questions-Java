<details>
  <summary>1. What are Classes </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In Java, a class is a blueprint or template for creating objects. It defines a data structure along with methods to operate on that data. Classes encapsulate the behavior and properties that objects of a certain type should have.</p>
</details>

<details>
  <summary>2. What are Objects </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Objects are instances of classes. They represent real-world entities and are created based on the structure defined by a class. Objects encapsulate data and the methods that operate on that data.</p>
</details>

<details>
  <summary>3. Mention the Use of OOP Concept</summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Object-Oriented Programming (OOP) is a programming paradigm that organizes code into objects. The use of OOP provides benefits such as code reusability, modularity, and the ability to model real-world entities more effectively through classes and objects.</p>
</details>

<details>
  <summary>4. What Ways Can We Create Objects in Java </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Objects in Java can be created in multiple ways:
    <ul>
      <li>Using the `new` keyword with a constructor.</li>
      <li>Using a static factory method.</li>
      <li>Using reflection.</li>
      <li>Using object cloning.</li>
    </ul>
  </p>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Example using the `new` keyword with a constructor:</p>
  
  ```java
  class MyClass {
      // Constructor
      public MyClass() {
          // Constructor logic goes here
      }
  }
  
  // Creating an object
  MyClass myObject = new MyClass();
  ```
</details>

<details>
  <summary>5. What Does `public static void main(String args[])` Mean </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">It is the entry point for Java applications. The `public static void main(String args[])` is a special method where the Java Virtual Machine (JVM) starts the execution of the program. It is mandatory in a standalone Java application.</p>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Example:</p>
  
  ```java
  public class MainClass {
      public static void main(String args[]) {
          // Application logic goes here
      }
  }
  ```
</details>

<details>
  <summary>6. What Is a Constructor </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">A constructor is a special method in a class that is invoked when an object of the class is created. It initializes the object's state and is used to perform tasks like allocating memory and setting default values. Constructors play a crucial role in the instantiation process of objects.</p>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Example:</p>
  
  ```java
  public class MyClass {
      // Default constructor
      public MyClass() {
          // Constructor logic goes here
      }
  
      // Parameterized constructor
      public MyClass(int value) {
          // Constructor logic with a parameter
      }
  }
  
  // Creating objects
  MyClass obj1 = new MyClass();          // Using the default constructor
  MyClass obj2 = new MyClass(10);        // Using the parameterized constructor
  ```
</details>

<details>
  <summary>7. What Is Destructor </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Unlike some other programming languages, Java does not have explicit destructors. Instead, Java relies on automatic garbage collection to reclaim memory occupied by objects that are no longer reachable or in use.</p>
</details>

<details>
  <summary>8. How to Create a Constructor </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">A constructor is created within a class by defining a method with the same name as the class. It does not have a return type, and it can take parameters for initializing the object's state. Here's an example:</p>
  
  ```java
  public class MyClass {
      public MyClass() {
          // Constructor logic goes here
      }
  }
  ```
</details>

<details>
  <summary>9. What Concepts Are There in OOP </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Key concepts in Object-Oriented Programming include:
    <ul>
      <li>Classes and Objects:< The basic building blocks of OOP.</li>
      <li>Inheritance:< A mechanism where a class can inherit properties and behaviors from another class.</li>
      <li>Polymorphism:< The ability of objects to take on multiple forms, achieved through method overloading and overriding.</li>
      <li>Abstraction:< The process of hiding complex implementation details and exposing only essential features.</li>
      <li>Encapsulation:< The bundling of data (attributes) and methods (functions) into a single unit known as a class.</li>
    </ul>
  </p>
</details>

<details>
  <summary>10. What Is Inheritance </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Inheritance is a fundamental concept in OOP where a class (subclass or derived class) inherits the properties and behaviors of another class (superclass or base class). It promotes code reusability and establishes an "is-a" relationship between classes.</p>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Example:</p>
  
  ```java
  // Superclass
  class Animal {
      void eat() {
          System.out.println("Animal is eating.");
      }
  }
  
  // Subclass inheriting from Animal
  class Dog extends Animal {
      void bark() {
          System.out.println("Dog is barking.");
      }
  }
  
  // Creating objects
  Animal myAnimal = new Animal();
  Dog myDog = new Dog();
  
  // Accessing inherited methods
  myAnimal.eat();   // Output: Animal is eating.
  myDog.eat();      // Output: Animal is eating. (inherited from Animal

)
myDog.bark(); // Output: Dog is barking.

````
</details>
<details>
<summary>11. What Is Polymorphism </summary>
<br>
<p style="background-color: #f2f2f2; margin-left: 20px;">Polymorphism allows objects of different types to be treated as objects of a common type. There are two types of polymorphism:</p>
<ul style="background-color: #f2f2f2; margin-left: 20px;">
<li>Compile-Time Polymorphism:< Achieved through method overloading where multiple methods have the same name but different parameters.</li>
<li>Runtime Polymorphism:< Achieved through method overriding where a subclass provides a specific implementation for a method defined in its superclass.</li>
</ul>
<p style="background-color: #f2f2f2; margin-left: 20px;">Example of Compile-Time Polymorphism:</p>

```java
class MathOperations {
  // Method to add two integers
  int add(int a, int b) {
      return a + b;
  }

  // Method to add three integers
  int add(int a, int b, int c) {
      return a + b + c;
  }
}

// Using Compile-Time Polymorphism
MathOperations mathObj = new MathOperations();
int result1 = mathObj.add(2, 3);         // Calls the first method
int result2 = mathObj.add(2, 3, 5);      // Calls the second method
````

  <p style="background-color: #f2f2f2; margin-left: 20px;">Example of Runtime Polymorphism:</p>
  
  ```java
  // Superclass
  class Shape {
      void draw() {
          System.out.println("Drawing a shape.");
      }
  }
  
  // Subclass overriding the draw method
  class Circle extends Shape {
      @Override
      void draw() {
          System.out.println("Drawing a circle.");
      }
  }
  
  // Using Runtime Polymorphism
  Shape myShape = new Circle();   // Reference of superclass, object of subclass
  myShape.draw();                // Calls the overridden draw method in Circle
  ```
</details>

<details>
  <summary>12.What Is Abstraction </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Abstraction is the process of hiding the complex implementation details and showing only the essential features of an object. Abstract classes and interfaces are used to achieve abstraction in Java.</p>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Example using an Abstract Class:</p>
  
  ```java
  // Abstract class
  abstract class Shape {
      // Abstract method (to be implemented by subclasses)
      abstract void draw();
  }
  
  // Concrete subclass implementing the abstract method
  class Circle extends Shape {
      @Override
      void draw() {
          System.out.println("Drawing a circle.");
      }
  }
  
  // Using abstraction
  Shape myShape = new Circle();   // Reference of abstract class, object of subclass
  myShape.draw();                // Calls the draw method in Circle
  ```
</details>

<details>
  <summary>13. What Is Encapsulation </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Encapsulation is the bundling of data (attributes) and methods (functions) that operate on the data into a single unit known as a class. It restricts direct access to some of the object's components, promoting data integrity and security.</p>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Example:</p>
  
  ```java
  public class BankAccount {
      private double balance;
  
      // Getter method to access the balance
      public double getBalance() {
          return balance;
      }
  
      // Setter method to update the balance
      public void setBalance(double newBalance) {
          if (newBalance >= 0) {
              balance = newBalance;
          }
      }
  }
  
  // Using encapsulation
  BankAccount myAccount = new BankAccount();
  myAccount.setBalance(1000.0);   // Setting the balance using the setter
  double currentBalance = myAccount.getBalance();  // Getting the balance using the getter
  ```
</details>

<details>
  <summary>14. What Are the Two Types of Polymorphism </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">The two types of polymorphism are:</p>
  <ul style="background-color: #f2f2f2; margin-left: 20px;">
    <li>Compile-Time Polymorphism:< It is achieved through method overloading where multiple methods have the same name but different parameters. The compiler determines which method to call based on the method signature.</li>
    <li>Runtime Polymorphism:< It is achieved through method overriding where a subclass provides a specific implementation for a method defined in its superclass. The decision on which method to call is made at runtime based on the actual object type.</li>
  </ul>
</details>

<details>
  <summary>15. What Are the Types of Inheritance in Java </summary>
  <br>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Types of inheritance in Java include:</p>
  <ul style="background-color: #f2f2f2; margin-left: 20px;">
    <li>Single Inheritance: A class can inherit from only one superclass.</li>
    <li>Multiple Inheritance (achieved through interfaces): A class can implement multiple interfaces, allowing it to inherit from more than one type.</li>
    <li>Multilevel Inheritance: A class can inherit from a class, and another class can inherit from it, forming a chain of inheritance.</li>
    <li>Hierarchical Inheritance: Multiple classes can inherit from a single superclass, forming a hierarchy of classes.</li>
  </ul>
</details>

<details>
  <summary>16. Can a Constructor be Inherited </summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">In object-oriented programming, a constructor is not inherited by subclasses. However, when a subclass is created, the constructor of its superclass is implicitly called to initialize the inherited members. This process is part of the subclass's instantiation but doesn't involve the direct inheritance of the constructor itself.</p>
</details>

<details>
  <summary>17. Can a Constructor be Overloaded </summary>
  <p style="background-color: #f2f2f2; margin-left: 20px;">Yes, constructors can be overloaded in Java. Constructor overloading involves defining multiple constructors for a class, each with a different parameter list. This allows objects of the class to be instantiated in different ways, providing flexibility and accommodating various initialization scenarios.</p>
</details>
<details>
  <summary>18. Explain different types of constructors in Java with examples </summary>

1. **Default Constructor:**
   A default constructor is one with no parameters. Java provides it automatically if a class doesn't define any constructors explicitly. It initializes the object with default values.

   ```java
   public class MyClass {
       // Default constructor provided by Java if not explicitly defined
   }

   // Instantiating an object using the default constructor
   MyClass obj = new MyClass();
   ```

2. **Parameterized Constructor:**
   A parameterized constructor includes parameters, allowing you to initialize the object with specific values provided during instantiation.

   ```java
   public class Person {
       String name;
       int age;

       // Parameterized constructor
       public Person(String n, int a) {
           name = n;
           age = a;
       }
   }

   // Instantiating an object using the parameterized constructor
   Person personObj = new Person("John", 25);
   ```

3. **Copy Constructor:**
   A copy constructor takes an object of the same class as a parameter and creates a new object with the same state. It is used to make a copy of an existing object.

   ```java
   public class Car {
       String model;
       int year;

       // Copy constructor
       public Car(Car otherCar) {
           model = otherCar.model;
           year = otherCar.year;
       }
   }

   // Creating an object and using the copy constructor
   Car originalCar = new Car();
   originalCar.model = "Toyota";
   originalCar.year = 2022;

   Car copiedCar = new Car(originalCar);
   ```

   </details>
