- [Basic](#basic)
  - [What is Java ?](#what-is-java-)
  - [Why use Java ?](#why-use-java-)
- [Java syntax](#java-syntax)
  - [Main method](#main-method)
    - [System.out.println()](#systemoutprintln)
- [Java output](#java-output)
  - [Print text](#print-text)
  - [Print numbers](#print-numbers)



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

## Main method 
The main() method is required and you will see it in every Java program :
```Java
// Main method 

   public static void main(String[] args)
```  
### System.out.println()
- Inside the main() method, we can use the `println()` method to print a line of text to the screen 
  ```Java
    public static void main(String[] args) {
      System.out.println("Hello World");
    }
  ```
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