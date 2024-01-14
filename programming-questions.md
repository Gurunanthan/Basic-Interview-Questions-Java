Certainly! Here are the formatted Java programs with explanations:

### 1. Hello World Program
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class HelloWorld {
      public static void main(String[] args) {
          System.out.println("Hello, World!");
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - A simple program that prints "Hello, World!" to the console.
  - `public class HelloWorld`: Declares a class named `HelloWorld`.
  - `public static void main(String[] args)`: The entry point of the program.
  - `System.out.println("Hello, World!");`: Prints the specified message to the console.
</details>

### 2. Calculate Sum of Two Numbers
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class SumOfTwoNumbers {
      public static void main(String[] args) {
          int num1 = 5, num2 = 7;
          int sum = num1 + num2;

          System.out.println("Sum of " + num1 + " and " + num2 + " is: " + sum);
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Calculates and prints the sum of two numbers (5 and 7).
  - `int num1 = 5, num2 = 7;`: Declares two integer variables.
  - `int sum = num1 + num2;`: Calculates the sum of `num1` and `num2`.
  - `System.out.println("Sum of " + num1 + " and " + num2 + " is: " + sum);`: Prints the result.
</details>

### 3. Find Area of a Rectangle
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class RectangleArea {
      public static void main(String[] args) {
          double length = 10.5, width = 5.5;
          double area = length * width;

          System.out.println("Area of the rectangle: " + area);
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Calculates and prints the area of a rectangle with length 10.5 and width 5.5.
  - `double length = 10.5, width = 5.5;`: Declares two double variables.
  - `double area = length * width;`: Calculates the area of the rectangle.
  - `System.out.println("Area of the rectangle: " + area);`: Prints the result.
</details>

### 4. Check if a Number is Even or Odd
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class EvenOrOdd {
      public static void main(String[] args) {
          int number = 8;

          if (number % 2 == 0) {
              System.out.println(number + " is even.");
          } else {
              System.out.println(number + " is odd.");
          }
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Checks and prints if a given number (8) is even or odd.
  - `int number = 8;`: Declares an integer variable.
  - `if (number % 2 == 0)`: Checks if the number is divisible by 2 (even).
  - `System.out.println(number + " is even.");`: Prints the result for even numbers.
  - `else`: Handles the case for odd numbers.
  - `System.out.println(number + " is odd.");`: Prints the result for odd numbers.
</details>

### 5. Calculate Factorial of a Number
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class Factorial {
      public static void main(String[] args) {
          int number = 5;
          long factorial = 1;

          for (int i = 1; i <= number; ++i) {
              factorial *= i;
          }

          System.out.println("Factorial of " + number + " = " + factorial);
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Calculates and prints the factorial of a number (5).
  - `int number = 5;`: Specifies the number for which the factorial is calculated.
  - `long factorial = 1;`: Initializes a variable to store the factorial.
  - Uses a `for` loop to calculate the factorial.
  - `System.out.println("Factorial of " + number + " = " + factorial);`: Prints the result.
</details>

### 6. Check Prime Number
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class PrimeNumber {
      public static void main(String[] args) {
          int number = 19;
          boolean isPrime = true;

          if (number <= 1) {
              isPrime = false;
          } else {
              for (int i = 2; i <= number / 2; ++i) {
                  if (number % i == 0) {
                      isPrime = false;
                      break;
                  }
              }
          }

          if (isPrime) {
              System.out.println(number + " is a prime number.");
          } else {
              System.out.println(number + " is not a prime number.");
          }
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Checks and prints if a given number (19) is a prime number.
  - `int number = 19;`: Declares an integer variable.
  - `boolean isPrime = true;`: Initializes a boolean variable to track primality.
  - Checks for numbers less than or equal to 1.
  - Uses a `for` loop to check divisibility up to half of the number.
  - `System.out.println(number + " is a prime number.");`: Prints the result for prime numbers.
  - `System.out.println(number + " is not a prime number.");`: Prints the result for non-prime numbers.
</details>

### 7. Reverse a String
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class ReverseString {
      public static void main(String[] args) {
          String original = "Hello, World!";
          String reversed = "";

          for (int i = original.length() - 1; i >= 0; --i) {
              reversed += original.charAt(i);
          }

          System.out.println("Original: " + original);
          System.out.println("Reversed: " + reversed);
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Reverses and prints a given string ("Hello, World!").
  - `String original = "Hello, World!";`: Declares a string variable.
  - `String reversed = "";`: Initializes an empty string to store the reversed version.


  - Uses a `for` loop to iterate over the characters in reverse order.
  - `reversed += original.charAt(i);`: Builds the reversed string.
  - Prints the original and reversed strings.
</details>

### 8. Swap Two Numbers
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class SwapNumbers {
      public static void main(String[] args) {
          int a = 5, b = 10;

          System.out.println("Before Swapping: a = " + a + ", b = " + b);

          int temp = a;
          a = b;
          b = temp;

          System.out.println("After Swapping: a = " + a + ", b = " + b);
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Swaps the values of two numbers (a = 5, b = 10).
  - `int a = 5, b = 10;`: Declare two integer variables.
  - `System.out.println("Before Swapping: a = " + a + ", b = " + b);`: Prints the values before swapping.
  - Swap the values using a temporary variable (`temp`).
  - `System.out.println("After Swapping: a = " + a + ", b = " + b);`: Prints the values after swapping.
</details>

### 9. Generate Fibonacci Series
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class FibonacciSeries {
      public static void main(String[] args) {
          int n = 10;
          int firstTerm = 0, secondTerm = 1;

          System.out.println("Fibonacci Series (First " + n + " terms):");

          for (int i = 1; i <= n; ++i) {
              System.out.print(firstTerm + ", ");
              int sum = firstTerm + secondTerm;
              firstTerm = secondTerm;
              secondTerm = sum;
          }
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Generates the Fibonacci series for the first 10 terms.
  - `int n = 10;`: Specifies the number of terms in the series.
  - `int firstTerm = 0, secondTerm = 1;`: Initialize the first two terms of the series.
  - `System.out.println("Fibonacci Series (First " + n + " terms):");`: Prints the message.
  - Uses a `for` loop to generate and print the Fibonacci series.
</details>

### 10. Check if a Year is a Leap Year
<details>
  <summary><strong>Program:</strong></summary>

  ```java
  public class LeapYear {
      public static void main(String[] args) {
          int year = 2024;
          boolean isLeapYear = false;

          if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
              isLeapYear = true;
          }

          if (isLeapYear) {
              System.out.println(year + " is a leap year.");
          } else {
              System.out.println(year + " is not a leap year.");
          }
      }
  }
  ```
</details>

<details>
  <summary><strong>Explanation:</strong></summary>

  - Checks and prints if a given year (2024) is a leap year.
  - `int year = 2024;`: Declares an integer variable.
  - `boolean isLeapYear = false;`: Initializes a boolean variable to track leap years.
  - Checks leap year conditions using an `if` statement.
  - `System.out.println(year + " is a leap year.");`: Prints the result for leap years.
  - `System.out.println(year + " is not a leap year.");`: Prints the result for non-leap years.
</details>