<div id="top-of-page"></div>

- [Java basics](#java-basics)
  - [What is java](#what-is-java)
  - [Programing language type](#programing-language-type)
  - [Highlevel programing language](#highlevel-programing-language)
  - [Lowlevel programing language](#lowlevel-programing-language)
      - [Structure of java](#structure-of-java)
      - [JDK Architecure](#jdk-architecure)
      - [Compiler](#compiler)
      - [JVM](#jvm)
- [Tokens in java program](#tokens-in-java-program)
        - [Datatypes](#datatypes)
        - [Premitive datatype](#premitive-datatype)
- [Printing statement of java](#printing-statement-of-java)
- [variable](#variable)
      - [output](#output)
      - [- steps to exicute a java program](#--steps-to-exicute-a-java-program)
  - [Structure of java](#structure-of-java-1)
      - [java keywords](#java-keywords)
    - [datatype](#datatype)
      - [system.out.println();](#systemoutprintln)
      - [variable](#variable-1)
  - [Constructor](#constructor)
  - [Object](#object)


# Java basics 
## What is java 
- java is easy to understand. 
- It is highlevel programing language.
- java provides a high security 
- java is platform indipendent 
- java consist of reach inbuild laibraries 
- java is object oriented programing language 
- java supports packages 
- java is robust (memory managementg) </br></br>

<div align="right"><a href="#top-of-page">(^)</a></div>

## Programing language type 
- Highlevel programing language
- lowlevel programing language
- middlelevel programing language
- ![Programming lang](<assets/images/programing lang jpg.JPG>)

<div align="right"><a href="#top-of-page">(^)</a></div>

## Highlevel programing language 
- The language which is writeable, readable, understandable and exicutable by a programer.
- ex - C, C++,Java etc.</br>

<div align="right"><a href="#top-of-page">(^)</a></div>

## Lowlevel programing language
- The language which is understandable and executable by the machine .
- ex - Binary language(0,1,0,1)</br>
    ( only one language in low level ).</br></br>

<div align="right"><a href="#top-of-page">(^)</a></div>

#### Structure of java 
- Structure of java consist two blocks 
   * class block
   * main method block
- in java the exicution of the program always starts from main method.</br></br>

<div align="right"><a href="#top-of-page">(^)</a></div>

#### JDK Architecure
  ![Github](<jdk architecture.JPG>)
- In JDK architecture some measure components are there like compiler and JVM 
- During the exicution of program JDK application will take some amount of memroy from 
  system and create an enviorment to exicute java program the enviorment is known as JRE 
- JRE consist of compiler and JVM </br></br>

<div align="right"><a href="#top-of-page">(^)</a></div>

#### Compiler
   ![Github](compiler.JPG)
- Compiler is a measure component of JDK which is used to read the java program line by line 
  and check for the errors inside it
- If the program is consisting any of the error either syntax or sementic the program will be
  given back to the programer by compiler 
- If the code is error free then it will be coverted into  byte code.</br></br>         

<div align="right"><a href="#top-of-page">(^)</a></div>

#### JVM
 ![Github](JVM.JPG)
- JVM stands for java vartual machine which is present inside jdk applications 
- JVM is not a physical component but gets invoke during program exicution 
- members of JVM are follows </br>
  * Interpreter 
  * class loader 
  * JVM memory daigram 
  * JIT
  * garbage collector
  * inbuild laibraries </br></br>

<div align="right"><a href="#top-of-page">(^)</a></div>

# Tokens in java program 
- Tokens is the smallest element in java program as it is a smallest members but plays a major role in every java program
- tokens are classified as follows</br>
    * keywords
    * Identifiers
    * literals
    * seprators
    * comments
    * operators</br></br>

<div align="right"><a href="#top-of-page">(^)</a></div>

##### Datatypes 
- Datatypes are the types of data which we are going to use in java program
- datatypes are completly depending on literals classified into two types 
     * Premitive datatype
     * Non Premitive datatype

<div align="right"><a href="#top-of-page">(^)</a></div>

##### Premitive datatype

  | Literals  |           | primitive datatype  | size                        |
  | --------- | --------- | ------------------- | --------------------------- |
  | Number    | integers  | byte short int long | 1 byte 2 byte 4 byte 8 byte |
  |           | float     | float double        | 4 byte 8 byte               |
  | character | character | char                | 2 byte                      |
  | boolean   | boolean   | boolean             | 1 bit                       | </br></br> |

<div align="right"><a href="#top-of-page">(^)</a></div>

# Printing statement of java 
  1. system.out.println ( ) ;
  1. system.out.print ( ) ;  

<div align="right"><a href="#top-of-page">(^)</a></div>

# variable 
- Variable it is a name given to a block of memory to store and access the value 
   - syntax :- </br>
               Datatype variable name = value ;</br>
               primitive - int -> wallet = 200 ;</br>
            non primitive - string -> = "apple" ;</br></br> 
-  We can create a variable for both primitive and non primitive datatype 
-  we can create two types of variable </br>
     * Global variable 
     * Local variable 
- Global variable are declared inside the class block 
- Local variable are declared inside the method block 
  ```Class p1 
     { 
       // global variable 
       public static voidmain(string []args)
       {
        // local variable
       }    
     }``` 
</br>

<div align="right"><a href="#top-of-page">(^)</a></div>

# java first program
- Example:
  ```java
  // my First Program
  class HelloWorld
  {
      public static void main(String[] args);
      {
          System.out.println("Hello, World!"); 
      }
  }
  /* Output: Hello, World! */
  ```
<div align="right"><a href="#top-of-page">(^)</a></div>

#### output
Hello, World! </br>

#### - steps to exicute a java program 
1. Create a source code
   - In order to create a ajava source code , we need to take the help of editors.
   - An editor it is a software which provides a platform to create a java source code.
   - ex - Notepad, visiual studio, notepad++, .txt,linux.

2. Compile source code 
   - To compile java source code we need to take the help of software by javac(java compiler)
   - we can acess javac by installing a software called JDK
   - The java compiler it will check for two types of error 
       1. Semantic error 
       2. Syntax error


3. Execute the byte code 

   - In order to execute a java byte code we need to acess a software called JRE ( JAVA RUNTIME ENVIORMENT ).
   - In order to acess JRE we need to install JDK software ( JAVA DEVLOPMENT KIT )

## Structure of java 
- structure of java consist of two blocks 
   1. class block 
   2. main method block 
- In java the exicution of the program always starts from main method </br>
   ``` 
   class  program name/class name  
   {
    public static void main( string[]args )
    {
      // main method
      system.out.println("shankarpalya"); 
    }
   } 
   ``` 

#### java keywords 
- keywords are the words whose meaining has already been explained to the java compiler .
   ![alt text](<java keywords.JPG>)   

###  datatype
- Datatypes are the types of data which we are going to use in java program .
- Datatypes are completly depending on literals classified into two types as follow :-
    1. primitive datatype 
    2. Non primitive datatype 

#### system.out.println();
- It is used to print a value and move the cursor to nextline
- For println statement passing a value is not a mandatory because it will still move the cursor to next new line 
- println statement works like line by line 
  ```
  main method
  {
    system.out.println();
    system.out.println("dog");
  }

#### system.out.print();
- print statement its work like word by word 
- for print statement passing a value is mandatory
  ```
  main method
   {
    system.out.print("how");
    system.out.print("are");
    system.out.print("you");
  }

  {
    system.out.print(); // CTE - compile time error

  }

#### variable 
- Variable it is a name given to block of memory to store and access the value.
- Syntax: 
  ```java
  datatype variable name = value;
  primitive int wallet = 200 ;
  non primitive string fruit = "apple";
  ```
- we can create a variable for both primitive and non primitive datatype
- we can create two types of variable 
   1. global variable
   2. local variable
- global variable are declared inside the class block 
- local variable are declared inside the method block 
  ```java
  class Person
  {
      // global variable
      public static void main(string []args)
      {
        // local variable 
      }
  }
### Local variable 
- local variable are declared inside the method block
- local variable does not consist any default values
- we can declare more value in local variable inside the method block but variable name as to be different 
- we can create a local variable for both primitive and non primitive datatype.
- Initialization for local variable is mandatory . 

### O+ Operator
- ' + ' operator we can use it for two ways 
- addition ( to perform addition both the data should be in number format )
- concate ( to merge anyone data should be in string formate )
   * int + int = int
   * int + float = float
   * int + char = int
   * float + float = float
   * char + char = int
   * float + char = float
   * int + string = string 
   * char + string = string 
   * float + string = string 
   * string + boolean = string 
   * string + string = string 
   * int + boolean = error 
   * char + boolean = error
   * float + boolean = error
   * boolean + boolean = error 
   * boolean + string = string 
  
#### primitive type custing 
- it is the process of converting one type of primitive data into another type of primitive data</br>

#### widening
- it is process of converting the value from small size datatype to large size datatype 


# Object Oriented Programming (OOP)

## Class
- It is important to remember that in Java, class names start with a **capital letter** and the file name should be saved as the class name.
- Syntax to create class
  ```java
  class Name{
    //methods
    //attributes
  }
  ```
- A class can contain-
  - Attributes
  - Methods
  - Constructors
  - Nested class
  - Interface

- **Access modifiers of class**
  - public
  - private
  - protected
  - default

- **Types of classes**
  - There are two types of classes-
    - **Built-in classes**:
      - The built-in classes are those which are pre-defined by the developers in JDK. 
    - **User-defined classes**
      - user-defined classes are the classes created by the user. 

<div align="right"><a href="#top-of-page">(^)</a></div>

## Constructor
- Every class has a constructor. 
- A constructor is a method that is used to initialize objects.
- Example:
  ```java
  class Person {
    constructor() {

    }
  }
  ```

<div align="right"><a href="#top-of-page">(^)</a></div>

## Object
- It is used to represent real-world entities that have a certain state, behavior, and identity. 
- They are known as ‘instance of a class’.
- The “new” keyword is used to allocate new memory space.
- Example:
  ```java
  class Classroom {
    int class_name;
    String lecture;
  }
  class Important{
    public static void main(String args[]){
      // creating object c1
      Classroom c1 = new Classroom();
      c1.class_name = 10;
      c1.lecture = "Java";
      System.out.println(c1.class_name+" "+c1.lecture);
    }
  }
  /* 
   Understand: We are trying to create object like below:
   c1 = {
    class_name: 10,
    lectures: "Java"
   }
  // Output: 10 Java
  ```

 // Object
  var class = {
    class_name: 10,
    lecture: 'java'
  }

 // Array
  var myArray = [1,2,3,4,5,6];
