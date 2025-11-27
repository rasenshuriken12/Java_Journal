# Java_Journal

<br> ![Author: Deviprasad Shetty](https://img.shields.io/badge/Author-💫_Deviprasad%20Shetty-000000?style=for-the-badge&labelColor=white)
<br> 

# My Intro:
<br> Hi, 😃👋 I'm Deviprasad Shetty, highly passionate for coding, learning and exploring new fields in Computer Science domain. 
<br> I'm excited 😃 to dive deeper into my technical skills, collaborate with others, and take on projects that challenge me to grow. 
<br> Always eager to learn and connect with others who share similar interests! 🤗🧑‍💻
<br> 
| [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5?style=for-the-badge&logo=LinkedIn&logoColor=white)](https://linkedin.com/in/deviprasad-shetty-4bba49313) | [![Website](https://img.shields.io/badge/Website-indigo?style=for-the-badge&logo=About.me&logoColor=white)](https://yourwebsite.com/) | [![My Portfolio](https://img.shields.io/badge/My_Portfolio-000?style=for-the-badge&logo=GitHub&logoColor=white)](https://github.com/DeviprasadShetty9833/DeviprasadShetty9833)  |                    
|---|---|---|

---
| [![Resources](https://img.shields.io/badge/📚_Back_to-Resources-A52A2A?style=for-the-badge&logo=book&logoColor=white)](https://github.com/DeviprasadShetty9833/Resources) |
|---|

---
# Java Basics

<table>
<tr><td>

⊡⁠ Java is a high-level, object-oriented, platform-independent programming language.

⊡⁠ Key Features:
- Write Once, Run Anywhere (WORA) thanks to JVM
- Strongly typed language with automatic memory management
- Robust and secure with exception handling
- Multi-threading support built-in


![Java](https://img.shields.io/badge/☕_1._-Print_a_Statement-E34F26?style=for-the-badge&logo=java&logoColor=white)

<details>
  <summary>Click to expand 🔻</summary>
    
*Code:*
```java
// HelloWorld.java                                   
public class HelloWorld {                          // Defines a class HelloWorld
    public static void main(String[] args) {       // Main method - program entry point
        System.out.println("Hello, Java World!");  // Function prints Output
    }
}
```

*Output:*
```
Hello, Java World!
```

> - System.out.println displays the string 'Hello, Java World!' on the console. `ln` after print adds new line
> - Java is case-sensitive: System ≠ system
> - curly braces {} are used to define blocks (scope) of code

</details>

![Java](https://img.shields.io/badge/☕_2._-Running_the_Java_code-E34F26?style=for-the-badge&logo=java&logoColor=white)

<details>
  <summary>Click to expand 🔻</summary>
  
- Write the above code in a code editor like VS Code / Intellij, Save it as `HelloWorld.java`
- Java Compiler `javac` compiles it into bytecode `HelloWorld.class`.
- JVM (Java Virtual Machine) reads the .class file and interprets the bytecode.
- JVM converts bytecode to machine readable code i.e. "binary" (001001010) and then execute the program.


| Type | Example Languages | How It Runs | 
|--|--|--|
| Compiled to machine code | C, C++, Rust | Directly executed by CPU | 
| Compiled to bytecode | **Java**, C# | Run on a virtual machine (JVM/CLR) | 
| Interpreted | Python, JavaScript | Executed line-by-line by an interpreter | 

</details>

![Java](https://img.shields.io/badge/☕_3._-Taking_User_Input-E34F26?style=for-the-badge&logo=java&logoColor=white)

<details> 
  <summary>Click to expand 🔻</summary>

*Code:*
```java
import java.util.Scanner;                         // Import Scanner class for input

public class UserInput {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        
        System.out.print("Enter your name: ");
        String name = s.nextLine();               // nextLine(): Reads entire line as String
        
        System.out.print("Enter your age: ");
        int age = s.nextInt();                    // nextInt(): Reads integer input
        
        System.out.print("Enter your salary: ");
        double salary = s.nextDouble();           // nextDouble(): Reads double input
        
        System.out.println("\n--- User Information ---");
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Salary: $" + salary);
        
        scanner.close();
    }
}
```

*Output:*
```
Enter your name: Naruto
Enter your age: 28
Enter your salary: 75000.50

--- User Information ---
Name: Naruto
Age: 28
Salary: $75000.5
```

> - Scanner scanner = new Scanner(System.in): Create scanner object
> - Always close scanner with scanner.close()

</details>

![Java](https://img.shields.io/badge/☕_4._-Comments-E34F26?style=for-the-badge&logo=java&logoColor=white)

<details>
  <summary>Click to expand 🔻</summary>
  
*Code:*
```java
// This is a comment

/*
This is a multi-line comment.
This is useful for explaining larger sections of code.
*/
```

*Output:*
```
```
</details>

</td></tr>
</table>

![Java](https://img.shields.io/badge/☕_4._-Data_Types-E34F26?style=for-the-badge&logo=java&logoColor=white)

*Code:*
```java
public class VariablesDemo {
    public static void main(String[] args) {
        // Primitive data types
        int age = 31;
        double salary = 50000.50;
        char grade = 'A';
        boolean isJavaFun = true;
        
        // Reference data type
        String name = "Kakashi Hatake";
        
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Salary: $" + salary);
        System.out.println("Grade: " + grade);
        System.out.println("Is Java Fun? " + isJavaFun);
    }
}
```

*Output:*
```
Name: Kakashi Hatake
Age: 31
Salary: $50000.5
Grade: A
Is Java Fun? true
```
- Java 25 Enhancement: You can use var for local variable type inference:
```java
var age = 31;                  // inferred as int
var name = "Kakashi Hatake";   // inferred as String
var salary = 50000.50;         // inferred as double
```

> - Primitive types: `int`, `double`, `char`, `boolean` - store actual values
> - Reference types: `String` - store reference to objects
> - `+` operator concatenates strings with other data types
    
## Multithreading

- Multithreading is a programming concept where a single program (process) runs multiple threads concurrently(not necessarily simultaneously).

- Process -	A running instance of a program. Has its own memory space, files, and resources.
- Thread - A smaller unit of execution within a process. Shares the same memory and resources with other threads of that process.
- Synchronization - Since threads share memory, two threads might try to modify the same variable at the same time, causing race conditions. Synchronization prevents this by allowing only one thread at a time to access a shared resource.
- Locking - Every object in Java has an internal lock. When a thread enters a synchronized block, it acquires the lock. Other threads must wait until it’s released.
- Deadlock - Occurs when two threads hold locks that each other needs — so neither proceeds.
- Race Conditions - When two or more threads access shared data without synchronization, results become unpredictable.

---

# Support:
If you like ❤️ this project, give it a ⭐ (Top right of page) and share it with friends!

---

| [![TOP](https://img.shields.io/badge/_🔺_-Navigate_to_TOP_↑_-blue?style=for-the-badge&labelColor=white)](#Java) | [![Website](https://img.shields.io/badge/Back_to-Website-indigo?style=for-the-badge&logo=About.me&logoColor=white)](https://yourwebsite.com/) |[![My Portfolio](https://img.shields.io/badge/Back_to-My_Portfolio-000?style=for-the-badge&logo=GitHub&logoColor=white)](https://github.com/DeviprasadShetty9833/DeviprasadShetty9833) |
|---|---|---|
