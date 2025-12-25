What is java?
- Java is programming language used to create software applications

Java History
- James gosling and team created the java language
- firstly created by sun microsystem now it is subsidiary of oracle
- developed in 1995
- first name was oak

Java Features
- Object Oriented
- Simple (Easy to learn syntax)
- Robust
- Security
- Multithreaded
- Portable
- Performance

Java is WORA (Write once run anywhere) language

Java Applications
- Standalone Applications (Desktop)
- Enterprise Applications
- Web Applications
- Mobile Applications
- Embedded System

Java Editions
- Java SE (Standard Edition)
- Java EE (Enterprise Edition)
- Java ME (Micro Edition)
- Java FX

Difference Between C++ and Java
C++
- Mainly used for system programming
- Support goto and operator overloading
- Does not support automatic garbage collection
- Platform dependent

Java
- Mainly used for to create software applications
- does not support goto and operator overloading
- Support automatic garbage collection
- Platform independent

Java Simple Program
public class Simple{
  public static void main(String args[]){
        System.out.println("Hello World");
        }
  }
}

class - used to declare class
main() - entry point of java program
static - no need to create object of simple to call main() method java will internally handle this
void - return type

Internal working of Java Program
Compile Time (for compiling we are using javac exe included under JDK)
- Java code will be converted to bytecode

Runtime
- class file -> classloader -> bytecode verifier -> interpreter
- classloader : Used to load the classes
    - Bootstrap Classloader
    - Extension Classloader
    - System/Applications Classloader
- bytecode verifier : Used to verify the bytecode any security related
- interpreter : will execute the bytecode into machine code (Execution Engine)

Can we save the java program with another name?
- Yes it is possible if the class is not public. while compile we have to used java file name but while executing on jvm we have to use class name only

Can we declared multiple classes in same class?
- Yes it is possible but all classes should be public only one class can be public and other should be without public

Difference between JDK, JRE, JVM
JDK (Java Development Kit)
- Provides development tools and JRE
- It physically exists
- Platform dependent

JRE (Java Runtime Environment)
- It is implementation of JVM, provides tools and other files that used while executing program at runtime
- It physically exists
- Contains JVM

JVM (Java Virtual Machine)
- It is an abstract machine(not physically exist) used to execute java bytecode into machine code
- platform dependent

Diagram

<img width="531" height="533" alt="Screenshot 2025-12-25 at 12 57 51 PM" src="https://github.com/user-attachments/assets/8404c1c7-b71b-4792-9c3f-a8a5c6883620" />

JVM architecture
- Class Loader
- Memory area
  - Heap : Used to store objects and primitive values
  - Stack : Used to store method execution stack and primitive refrences
  - Class Area : Used to store class related information
- Execution engine
  - Interpreter
  - JIT comipler (to improve the performance of interpreter)
  - Garbage collection

Java Variables
- Variables are the container to used to store values
- Types of variables
  - Instance variable (related to class level using object we can access this)
  - Local variable (inside method body can't access outside the method body)
  - Static variable (related to class level declare using static keyword no need to create object to access using class name and this keyword we can access variable)

Java Datatypes
- Primitive Datatypes
  - int (default value 0)
  - char 
  - long (default value 0)
  - double (default value 
  - short
  - byte
  - float (default value 0.0)
  - boolean (default value false)

- Non-Primitive Datatypes
  - String
  - Arrays
  - Classes
  - Objects
  - Enum

Better for memory management.






  
