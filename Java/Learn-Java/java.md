- [Basic](#basic)
  - [What is Java ?](#what-is-java-)
  - [Why use Java ?](#why-use-java-)
- [Java syntax](#java-syntax)
  - [Main method](#main-method)
    - [System.out.println()](#systemoutprintln)
- [Java output](#java-output)
  - [Print text](#print-text)
  - [Print numbers](#print-numbers)
- [Java Comments](#java-comments)
  - [Single line comment](#single-line-comment)
  - [Multi line comments](#multi-line-comments)
- [Java variables](#java-variables)
  - [Types of variables in java](#types-of-variables-in-java)
    - [Java print variables](#java-print-variables)
  - [**Java Identifiers**](#java-identifiers)
- [Java Data Types](#java-data-types)
  - [**Primitive Data Types**](#primitive-data-types)
  - [Java Numbers](#java-numbers)
  - [Integer Types](#integer-types)
  - [**Floating Point Types**](#floating-point-types)
  - [Scientific Numbers](#scientific-numbers)
  - [Java Boolean Data Types](#java-boolean-data-types)
  - [Java Characters](#java-characters)
    - [String](#string)
- [Java Type Casting](#java-type-casting)
  - [**Widening casting**](#widening-casting)
  - [**Narrowing Casting**](#narrowing-casting)
- [Java operators](#java-operators)



# Basic 
## What is Java ?
- java is easy to understand. 
- It is high-level programming language.
- java provides a high security 
- java is platform independent 
- java consist of reach in-build laibraries 
- java is object oriented programming language 
- java supports packages 
- java is robust (memory management)

<p align="right">(<a href="#top">˄</a>)</p>

## Why use Java ?
- Java works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc.)
- It is one of the most popular programming languages in the world
- It has a large demand in the current job market
- It is easy to learn and simple to use
- It is open-source and free
- It is secure, fast and powerful
- It has huge community support (tens of millions of developers)
- Java is an object oriented language which gives a clear structure to programs and allows code to be reused, lowering development costs
- As Java is close to C++ and C#, it makes it easy for programmers to switch to Java

<p align="right">(<a href="#top">˄</a>)</p>

# Java syntax
```Java 
 // Main.java

   public class Main {
      public static void main(String[] args) {
        System.out.println("Hello World");
      }
    }
```  
Every line of code that runs in Java must be inside a class. In our example, we named the class Main. A class should always start with an uppercase first letter.

- **Note** : Java is case-sensitive : `"MyClass"` and `"myclass"` has different meaning.
  
  <p align="right">(<a href="#top">˄</a>)</p>

## Main method 
The main() method is required and you will see it in every Java program :
```Java
// Main method 

   public static void main(String[] args)
```  
<p align="right">(<a href="#top">˄</a>)</p>

### System.out.println()
- Inside the main() method, we can use the `println()` method to print a line of text to the screen 
  ```Java
    public static void main(String[] args) {
      System.out.println("Hello World");
    }
  ```
  <p align="right">(<a href="#top">˄</a>)</p>

# Java output
## Print text
 - we can use the println() method to output values or print text in Java :
 - **example**
  ```java
    System.out.println("Hello World!");
  ```  
## Print numbers 
- we you can also use the println() method to print numbers.
- However, unlike text, we don't put numbers inside double quotes:

- **Example**
   ```java
      System.out.println(3);
      System.out.println(358);
      System.out.println(50000);
   ```
  - You can also perform mathematical calculations inside the println() method:
   ```java
      System.out.println(3 + 3);
   ```  
   ```java
      System.out.println(2 * 5);
   ```   
   <p align="right">(<a href="#top">˄</a>)</p>

# Java Comments 
 - Comments can be used to explain Java code, and to make it more readable. It can also be used to prevent execution when testing alternative code.

## Single line comment
 - Single-line comments start with two forward slashes `(//)`.

 - Any text between `//` and the end of the line is ignored by Java (will not be executed). 
 - **Example**
    ```java
      // This is a comment
      System.out.println("Hello World");
    ```  
## Multi line comments
 - Multi-line comments start with `/*` and ends with `*/`.

 - Any text between `/*` and `*/` will be ignored by Java.    
   ```java
       /* The code below will print the words Hello World
        to the screen, and it is amazing */
      System.out.println("Hello World");
   ```
   <p align="right">(<a href="#top">˄</a>)</p>

# Java variables 
**Variables are containers for storing data values.**   

## Types of variables in java 
1. **Local Variables** :
     -  These variables are created when the block is entered, or the function is called and destroyed after exiting from the block or when the call returns from the function.
     - The scope of these variables exists only within the block in which the variables are declared, i.e., we can access these variables only within that block.
     - Initialization of the local variable is mandatory before using it in the defined scope.
  - **Example**
     ```java
        // Java Program to implement
      // Local Variables
      import java.io.*;

      class GFG {
        public static void main(String[] args)
        {
          // Declared a Local Variable
          int var = 10;

          // This variable is local to this main method only
          System.out.println("Local Variable: " + var);
        }
      }
    ```
    - **Example**
    ```java
      package a;
      public class LocalVariable {
        public static void main(String[] args)
        {
          // x is a local variable
          int x = 10;

          // message is also a local
          // variable
          String message = "Hello, world!";

          System.out.println("x = " + x);
          System.out.println("message = " + message);

          if (x > 5) {
            // result is a
            // local variable
            String result = "x is greater than 5";
            System.out.println(result);
          }

          // Uncommenting the line below will result in a
          // compile-time error System.out.println(result);

          for (int i = 0; i < 3; i++) {
            String loopMessage
              = "Iteration "
              + i; // loopMessage is a local variable
            System.out.println(loopMessage);
          }

          // Uncommenting the line below will result in a
          // compile-time error
          // System.out.println(loopMessage);
        }
      }

    ```    
<p align="right">(<a href="#top">˄</a>)</p>

2. **Instance Variables** : 
     - As instance variables are declared in a class, these variables are created when an object of the class is created and destroyed when the object is destroyed.
    - Unlike local variables, we may use access specifiers for instance variables. If we do not specify any access specifier, then the default access specifier will be used.
    - Initialization of an instance variable is not mandatory. Its default value is dependent on the data type of variable. For String it is null, for float it is 0.0f, for int it is 0, for Wrapper classes like Integer it is null, etc.
    - Instance variables can be accessed only by creating objects.
    - We initialize instance variables using constructors while creating an object. We can also use instance blocks to initialize the instance variables.
- **Example**
   ```java 
     // Java Program to demonstrate
      // Instance Variables
      import java.io.*;

      class GFG {

        // Declared Instance Variable
        public String geek;
        public int i;
        public Integer I;
        public GFG()
        {
          // Default Constructor
          // initializing Instance Variable
          this.geek = "Name";
        }

        // Main Method
        public static void main(String[] args)
        {
          // Object Creation
          GFG name = new GFG();

          // Displaying O/P
          System.out.println("Geek name is: " + name.geek);
          System.out.println("Default value for int is "
                  + name.i);
        
          // toString() called internally
          System.out.println("Default value for Integer is "
                  + name.I);
        }
      }
   ```
   <p align="right">(<a href="#top">˄</a>)</p>

1. **Static Variables**
     - These variables are declared similarly to instance variables. The difference is that static variables are declared using the static keyword within a class outside of any method, constructor, or block.
     - Unlike instance variables, we can only have one copy of a static variable per class, irrespective of how many objects we create.
     - Static variables are created at the start of program execution and destroyed automatically when execution ends.
     - Initialization of a static variable is not mandatory. Its default value is dependent on the data type of variable. For String it is null, for float it is 0.0f, for int it is 0, for Wrapper classes like Integer it is null, etc.
- **Example**
  ```java
  // Java Program to demonstrate
    // Static variables
    import java.io.*;

    class GFG {
      // Declared static variable
      public static String geek = "Shubham Jain";

      public static void main(String[] args)
      {

        // geek variable can be accessed without object
        // creation Displaying O/P GFG.geek --> using the
        // static variable
        System.out.println("Geek Name is : " + GFG.geek);

        // static int c=0;
        // above line,when uncommented,
        // will throw an error as static variables cannot be
        // declared locally.
      }
    }

  ```
  <p align="right">(<a href="#top">˄</a>)</p>

### Java print variables 
 - **Display Variables**
     - The println() method is often used to display variables.

     - To combine both text and a variable, use the + character  
 - **Example**
   ```java
   String name = "John";
     // (+ character)
   System.out.println(" Hello " + name);
   ```
  - You can also use the + character to add a variable to another variable:
  - **Example**
  ```java
      String firstName = "John ";
      String lastName = "Doe";
      String fullName = firstName + lastName;
      System.out.println(fullName);
  ```
- **Declare Many Variables**
  - To declare more than one variable of the same type, you can use a comma-separated list:
  ```java
     int x = 5, y = 6, z = 50;
     System.out.println(x + y + z);
  ```
- **One Value to Multiple Variables**
  - You can also assign the same value to multiple variables in one line:
  ```java
     int x, y, z;
     x = y = z = 50;
     System.out.println(x + y + z);
  ```     
  <p align="right">(<a href="#top">˄</a>)</p>

## **Java Identifiers**
   - All Java variables must be identified with unique names.

   - These unique names are called identifiers.

   - Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
   
  - **Example**
   ```java
      // Good
      int minutesPerHour = 60;

      // OK, but not so easy to understand what m actually is
     int m = 60;
   ```
<p align="right">(<a href="#top">˄</a>)</p>

# Java Data Types

- Data types are divided into two groups:
  - **Primitive data types** - includes `byte`, `short`, `int`, `long`, `float`, `double`, `boolean` and `char`.
  
  - **Non-primitive data types** - such as `String`, `Arrays` and `Classes`. 
  - 
<p align="right">(<a href="#top">˄</a>)</p>

## **Primitive Data Types**
- A primitive data type specifies the size and type of variable values, and it has no additional methods.
- There are eight primitive data types in Java:
  <img src="assets/images/data types.JPG">

- **Non - primitive data type**
  - Non-primitive data types in Java are not predefined. They are created by the programmer. Non-primitive data types are also called 'reference variables' or 'object references' as they reference a memory location where data is stored.
  
<p align="right">(<a href="#top">˄</a>)</p>

## Java Numbers 
  Primitive number types are divided into two groups:

- **Integer types** stores whole numbers, positive or negative (such as 123 or -456), without decimals. Valid types are byte, short, int and long. Which type you should use, depends on the numeric value.
- **Floating point** types represents numbers with a fractional part, containing one or more decimals. There are two types: float and double.

## Integer Types
1. **byte** : The byte data type can store whole numbers from -128 to 127. This can be used instead of int or other integer types to save memory when you are certain that the value will be within -128 and 127:
   ```java
      byte myNum = 100;
      System.out.println(myNum); 
   ```

2. **Short** : The short data type can store whole numbers from -32768 to 32767:  
   ```java
      short myNum = 5000;
      System.out.println(myNum);
   ```
3. **int** : The int data type can store whole numbers from -2147483648 to 2147483647. In general, and in our tutorial, the int data type is the preferred data type when we create variables with a numeric value.
   ```java
      int myNum = 100000;
      System.out.println(myNum);
   ```   
4. **Long** : The long data type can store whole numbers from -9223372036854775808 to 9223372036854775807. This is used when int is not large enough to store the value. Note that you should end the value with an "L":
    ```java
       long myNum = 15000000000L;
       System.out.println(myNum);
    ```   
    <p align="right">(<a href="#top">˄</a>)</p>

 ## **Floating Point Types** 
  - You should use a floating point type whenever you need a number with a decimal, such as 9.99 or 3.14515.

- The float and double data types can store fractional numbers. Note that you should end the value with an " f " for floats and " d " for doubles:

```java
   // float example 
      float myNum = 5.75f;
     System.out.println(myNum);
```
```java
   // double example
   double myNum = 19.99d;
  System.out.println(myNum);
```
<p align="right">(<a href="#top">˄</a>)</p>

## Scientific Numbers
 - A floating point number can also be a scientific number with an "e" to indicate the power of 10:
```java
    float f1 = 35e3f;
    double d1 = 12E4d;
    System.out.println(f1);
    System.out.println(d1);
```
<p align="right">(<a href="#top">˄</a>)</p>

## Java Boolean Data Types
 Boolean Types :
 - Very often in programming, you will need a data type that can only have one of two values, like:

   - YES / NO
   - ON / OFF
   - TRUE / FALSE
- For this, Java has a boolean data type, which can only take the values true or false:
- **Example**
```java
  boolean isJavaFun = true;
  boolean isFishTasty = false;
  System.out.println(isJavaFun);     // Outputs true
  System.out.println(isFishTasty);   // Outputs false  
```
<p align="right">(<a href="#top">˄</a>)</p>

## Java Characters
- The char data type is used to store a single character. The character must be surrounded by single quotes, like 'A' or 'c':
- **Example**
```java
  char myGrade = 'B';
  System.out.println(myGrade);
```
Alternatively, if you are familiar with ASCII values, you can use those to display certain characters:
```java
  char myVar1 = 65, myVar2 = 66, myVar3 = 67;
  System.out.println(myVar1);    // a
  System.out.println(myVar2);    // b
  System.out.println(myVar3);    // c
```
<p align="right">(<a href="#top">˄</a>)</p>

### String 
- The String data type is used to store a sequence of characters (text). String values must be surrounded by double quotes:
```java 
 String greeting = "Hello World";
 System.out.println(greeting);
```
# Java Type Casting
- Type casting is when you assign a value of one primitive data type to another type.
- In Java, there are two types of casting:
    - Widening Casting (automatically) - converting a smaller type to a larger type size
 `byte` -> `short` -> `char` -> `int` -> `long` -> `float` -> `double`
   
   - Narrowing Casting (manually) - converting a larger type to a smaller size type
`double` -> `float` -> `long` -> `int` -> `char` -> `short` -> `byte`

<p align="right">(<a href="#top">˄</a>)</p>

## **Widening casting** 
- Widening casting is done automatically when passing a smaller size type to a larger size type:
- **Example**
```java
  public class Main {
    public static void main(String[] args) {
      int myInt = 9;
      double myDouble = myInt; // Automatic casting: int to double

      System.out.println(myInt);      // Outputs 9
      System.out.println(myDouble);   // Outputs 9.0
    }
  } 
```
<p align="right">(<a href="#top">˄</a>)</p>

## **Narrowing Casting**
- Narrowing casting must be done manually by placing the type in parentheses in front of the value:
- **Example**
```java
  public class Main {
    public static void main(String[] args) {
      double myDouble = 9.78d;
      int myInt = (int) myDouble; // Manual casting: double to int

      System.out.println(myDouble);   // Outputs 9.78
      System.out.println(myInt);      // Outputs 9
    }
  }
```
<p align="right">(<a href="#top">˄</a>)</p>

# Java operators
- Operators are used to perform operations on variables and values.
- **Example**
```java
  int x = 100 + 50;  // + operator to add together two values
```
-  it can also be used to add together a variable and a value, or a variable and another variable:  
```java
  int sum1 = 100 + 50;        // 150 (100 + 50)
  int sum2 = sum1 + 250;      // 400 (150 + 250)
  int sum3 = sum2 + sum2;     // 800 (400 + 400)
```
- Java divides the operators into the following groups:

   - Arithmetic operators
   - Assignment operators
   - Comparison operators
   - Logical operators
   - Bitwise operators

- **Arithmetic operators** : Arithmetic operators are used to perform common mathematical operations.
  <img src="assets/images/arithmetic operators.JPG">

- **Java Assignment Operators** :Assignment operators are used to assign values to variables.
- **Example**
```java
  //  we use the assignment operator (=) to assign the value 10 to a variable called x:
  int x = 10;
```