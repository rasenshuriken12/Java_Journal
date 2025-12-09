# Java_Journal

| ![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5?style=for-the-badge&logo=LinkedIn&logoColor=white) | [![My_Portfolio](https://img.shields.io/badge/My_Portfolio-indigo?style=for-the-badge&logo=firefox&logoColor=white)](https://yourwebsite.com/) | [![GitHub](https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=GitHub&logoColor=white)](https://github.com/rasenshuriken12/rasenshuriken12)  |
|---|---|---|

---

| [![Resources](https://img.shields.io/badge/📚_Back_to-Resources-A52A2A?style=for-the-badge&logo=book&logoColor=white)](https://github.com/rasenshuriken12/Resources) |
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



Java Programs:

<table>
<tr><td>

<br> ⊡⁠ Java is a versatile, object-oriented programming language known for its "Write Once, Run Anywhere" capability
<br> ⊡⁠ Key Features:
- Platform independence through JVM
- Strong typing and automatic memory management
- Rich standard library and ecosystem
- Multithreading support built-in

<br> ![1.](https://img.shields.io/badge/_1._-Simple%20Java%20Program-007396?style=for-the-badge&logo=java&logoColor=white)   

<details>
  <summary>Click to expand 🔻</summary>

Code:

```java
public class Example {
    public static void main(String[] args) {
        System.out.println("This is a simple Java program.");
    }
}
```

Output:

```
This is a simple Java program.
```

· public class Example: Every Java program is a class. The class name must match the filename
· public static void main(String[] args): The entry point of every Java application
· System.out.println(): Prints text to console and moves to next line
· Curly braces {} define code blocks
· Semicolon ; ends each statement

Java 25 Note: This basic structure remains unchanged in all Java versions.

</details>

<br> ![2.](https://img.shields.io/badge/_2._-Variables%20and%20Printing-007396?style=for-the-badge&logo=java&logoColor=white)   

<details>
  <summary>Click to expand 🔻</summary>

Code:

```java
public class Example2 {
    public static void main(String[] args) {
        int num;
        num = 100;
        
        System.out.println("This is num: " + num);
        
        num = num * 2;
        
        System.out.print("The value of num * 2 is ");
        System.out.println(num);
    }
}
```

Output:

```
This is num: 100
The value of num * 2 is 200
```

· int num;: Declares an integer variable named 'num'
· num = 100;: Assigns value 100 to the variable
· num = num * 2;: Multiplies current value by 2 and stores result back
· System.out.print(): Prints without newline
· System.out.println(): Prints with newline
· + operator concatenates strings with variables

Java 25 Enhancement: You can use var for cleaner variable declaration:

```java
var num = 100;  // Type inferred as int
```

</details>

<br> ![3.](https://img.shields.io/badge/_3._-If%20Statement%20Demo-007396?style=for-the-badge&logo=java&logoColor=white)   

<details>
  <summary>Click to expand 🔻</summary>

Code:

```java
public class IfSample {
    public static void main(String[] args) {
        int x, y;
        x = 10;
        y = 20;
        
        if (x < y) 
            System.out.println("x is less than y");
        
        x = x * 2;
        
        if (x == y) 
            System.out.println("x now equal to y");
        
        x = x * 2;
        if (x > y) 
            System.out.println("x now greater than y");
        
        if (x == y) 
            System.out.println("you won't see this");
    }
}
```

Output:

```
x is less than y
x now equal to y
x now greater than y
```

· int x, y;: Declares multiple variables of same type
· if (condition): Executes code block only if condition is true
· Comparison operators: < (less than), == (equal to), > (greater than)
· When x=10, y=20: x < y is true
· When x=20, y=20: x == y is true
· When x=40, y=20: x > y is true
· Last condition (x == y) is false, so message not printed

Java 25 Note: If statements work identically. Consider using braces {} for better readability.

</details>

---

Now let me continue with the next three programs:

<br> ![4.](https://img.shields.io/badge/_4._-For%20Loop%20Demo-007396?style=for-the-badge&logo=java&logoColor=white)   

<details>
  <summary>Click to expand 🔻</summary>

Code:

```java
public class ForTest {
    public static void main(String[] args) {
        int x;
        
        for (x = 0; x < 10; x = x + 1)
            System.out.println("This is x: " + x);
    }
}
```

Output:

```
This is x: 0
This is x: 1
This is x: 2
This is x: 3
This is x: 4
This is x: 5
This is x: 6
This is x: 7
This is x: 8
This is x: 9
```

· for (initialization; condition; increment): Standard for loop structure
· x = 0: Initializes counter variable
· x < 10: Loop continues while this condition is true
· x = x + 1: Increments counter after each iteration (can also use x++)
· Loop runs 10 times (x values 0 through 9)
· When x becomes 10, condition fails and loop exits

Java 25 Enhancement: Modern for loop syntax:

```java
for (int x = 0; x < 10; x++) {
    System.out.println("This is x: " + x);
}
```

</details>

<br> ![5.](https://img.shields.io/badge/_5._-Code%20Blocks%20Demo-007396?style=for-the-badge&logo=java&logoColor=white)   

<details>
  <summary>Click to expand 🔻</summary>

Code:

```java
public class BlockTest {
    public static void main(String[] args) {
        int x, y;
        y = 20;
        
        for (x = 0; x < 10; x++) {
            System.out.println("This is x: " + x);
            System.out.println("This is y: " + y);
            y = y - 2;
        }
    }
}
```

Output:

```
This is x: 0
This is y: 20
This is x: 1
This is y: 18
This is x: 2
This is y: 16
...
This is x: 9
This is y: 2
```

· Code block {...} groups multiple statements together
· All statements inside block execute for each loop iteration
· x++ is shorthand for x = x + 1 (increment)
· y = y - 2 decreases y by 2 each iteration
· x increases from 0 to 9, y decreases from 20 to 2
· Shows how multiple variables can change within a loop

Java 25 Note: Code blocks work the same way. Using blocks with loops is recommended practice.

</details>

<br> ![6.](https://img.shields.io/badge/_6._-Light%20Distance%20Calculation-007396?style=for-the-badge&logo=java&logoColor=white)   

<details>
  <summary>Click to expand 🔻</summary>

Code:

```java
public class Light {
    public static void main(String[] args) {
        int lightspeed;
        long days, seconds, distance;
        
        lightspeed = 186000;
        days = 1000;
        
        seconds = days * 24 * 60 * 60;
        distance = lightspeed * seconds;
        
        System.out.print("In " + days);
        System.out.print(" days light will travel about ");
        System.out.println(distance + " miles.");
    }
}
```

Output:

```
In 1000 days light will travel about 16070400000000 miles.
```

· Uses long data type for large numbers that exceed int range
· lightspeed: Speed of light (186,000 miles/second)
· seconds = days * 24 * 60 * 60: Converts days to seconds
· distance = lightspeed * seconds: Distance = speed × time
· System.out.print() used for continuous output on same line
· Demonstrates mathematical calculations with different data types

Java 25 Enhancement: You can use underscores in large numbers for readability:

```java
int lightspeed = 186_000;
long distance = 16_070_400_000_000L;
```

</details>

---



    
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

| [![TOP](https://img.shields.io/badge/_🔺_-Navigate_to_TOP_↑_-blue?style=for-the-badge&labelColor=white)](#Java) | [My_Portfolio](https://img.shields.io/badge/My_Portfolio-indigo?style=for-the-badge&logo=firefox&logoColor=white)](https://yourwebsite.com/) | [![GitHub](https://img.shields.io/badge/Back_to-Github-000?style=for-the-badge&logo=GitHub&logoColor=white)](https://github.com/rasenshuriken12/rasenshuriken12) |
|---|---|---|
