# Java in Minutes

<aside>
👨🏻‍🏫 Quick Revision

</aside>

### Lesson 1: The Basic Structure of a Java Program

A simple Java program consists of at least one class and a `main` method. Let's start with the most basic Java program:

```java
javaCopy code
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}

```

### Explanation:

1. **public class HelloWorld**: This defines a class named `HelloWorld`. In Java, every application must have at least one class.
2. **public static void main(String[] args)**: This is the `main` method, which is the entry point of any Java application. The JVM looks for this method to start the program.
3. **System.out.println("Hello, World!");**: This line prints the text "Hello, World!" to the console.

### Exercise 1:

1. Open a text editor or an Integrated Development Environment (IDE) like IntelliJ IDEA or Eclipse.
2. Copy the above code into a new file named `HelloWorld.java`.
3. Compile the program using `javac HelloWorld.java` and run it using `java HelloWorld` in the terminal.

### Lesson 2: Variables and Data Types

Variables store data that can be used and manipulated in your program. Let's learn about different data types and how to declare variables.

```java
javaCopy code
public class VariablesExample {
    public static void main(String[] args) {
        int number = 10;                // Integer (whole number)
        double price = 19.99;           // Floating point number
        char letter = 'A';              // Character
        boolean isJavaFun = true;       // Boolean (true/false)
        String greeting = "Hello";      // String (sequence of characters)

        System.out.println("Number: " + number);
        System.out.println("Price: " + price);
        System.out.println("Letter: " + letter);
        System.out.println("Is Java Fun: " + isJavaFun);
        System.out.println("Greeting: " + greeting);
    }
}

```

### Explanation:

1. **int number = 10;**: Declares an integer variable named `number` and initializes it to 10.
2. **double price = 19.99;**: Declares a double variable named `price` and initializes it to 19.99.
3. **char letter = 'A';**: Declares a char variable named `letter` and initializes it to 'A'.
4. **boolean isJavaFun = true;**: Declares a boolean variable named `isJavaFun` and initializes it to true.
5. **String greeting = "Hello";**: Declares a String variable named `greeting` and initializes it to "Hello".

### Exercise 2:

1. Create a new file named `VariablesExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.

### Lesson 3: Basic Operations

Now, let's learn how to perform basic arithmetic operations.

```java
javaCopy code
public class BasicOperations {
    public static void main(String[] args) {
        int a = 10;
        int b = 5;

        int sum = a + b;         // Addition
        int difference = a - b;  // Subtraction
        int product = a * b;     // Multiplication
        int quotient = a / b;    // Division
        int remainder = a % b;   // Modulus (remainder)

        System.out.println("Sum: " + sum);
        System.out.println("Difference: " + difference);
        System.out.println("Product: " + product);
        System.out.println("Quotient: " + quotient);
        System.out.println("Remainder: " + remainder);
    }
}

```

### Explanation:

1. **int sum = a + b;**: Adds `a` and `b`, and stores the result in `sum`.
2. **int difference = a - b;**: Subtracts `b` from `a`, and stores the result in `difference`.
3. **int product = a * b;**: Multiplies `a` and `b`, and stores the result in `product`.
4. **int quotient = a / b;**: Divides `a` by `b`, and stores the result in `quotient`.
5. **int remainder = a % b;**: Calculates the remainder when `a` is divided by `b`, and stores the result in `remainder`.

### Exercise 3:

1. Create a new file named `BasicOperations.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.

### Lesson 4: Control Structures - If Statements

Control structures allow you to control the flow of your program. Let's start with `if` statements.

```java
javaCopy code
public class IfStatements {
    public static void main(String[] args) {
        int number = 10;

        if (number > 0) {
            System.out.println("The number is positive.");
        } else if (number < 0) {
            System.out.println("The number is negative.");
        } else {
            System.out.println("The number is zero.");
        }
    }
}

```

### Explanation:

1. **if (number > 0)**: Checks if `number` is greater than 0.
2. **else if (number < 0)**: If the previous condition is false, checks if `number` is less than 0.
3. **else**: If none of the above conditions are true, this block is executed.

### Exercise 4:

1. Create a new file named `IfStatements.java`.
2. Copy the above code into this file.
3. Change the value of `number` and observe how the output changes.
4. Compile and run the program to see the output.

### Lesson 5: Loops

Loops allow you to execute a block of code multiple times. Let's start with `for` loops and `while` loops.

### For Loop

A `for` loop is useful when you know in advance how many times you want to execute a statement or a block of statements.

```java
javaCopy code
public class ForLoopExample {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            System.out.println("i is: " + i);
        }
    }
}

```

### Explanation:

1. **for (int i = 0; i < 5; i++)**: Initializes `i` to 0, checks if `i` is less than 5, and increments `i` by 1 after each iteration.
2. **System.out.println("i is: " + i);**: Prints the value of `i`.

### Exercise 5.1:

1. Create a new file named `ForLoopExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.

### While Loop

A `while` loop is useful when you want to repeat a block of code as long as a condition is true.

```java
javaCopy code
public class WhileLoopExample {
    public static void main(String[] args) {
        int i = 0;
        while (i < 5) {
            System.out.println("i is: " + i);
            i++;
        }
    }
}

```

### Explanation:

1. **int i = 0;**: Initializes `i` to 0.
2. **while (i < 5)**: Checks if `i` is less than 5.
3. **System.out.println("i is: " + i);**: Prints the value of `i`.
4. **i++;**: Increments `i` by 1.

### Exercise 5.2:

1. Create a new file named `WhileLoopExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.

### Lesson 6: Methods

Methods are reusable blocks of code that perform a specific task. They help you organize your code and make it more readable and maintainable.

```java
javaCopy code
public class MethodsExample {
    public static void main(String[] args) {
        printHello();
        int result = add(5, 3);
        System.out.println("Sum: " + result);
    }

    // Method to print a message
    public static void printHello() {
        System.out.println("Hello!");
    }

    // Method to add two numbers and return the result
    public static int add(int a, int b) {
        return a + b;
    }
}

```

### Explanation:

1. **printHello()**: This method prints "Hello!" to the console.
2. **add(int a, int b)**: This method takes two integers as parameters, adds them, and returns the result.

### Exercise 6:

1. Create a new file named `MethodsExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try adding more methods to perform different operations, like subtraction, multiplication, etc.

### Lesson 7: Classes and Objects

In Java, classes are blueprints for creating objects. An object is an instance of a class. Let's create a simple class and create objects from it.

```java
javaCopy code
class Person {
    String name;
    int age;

    // Constructor
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Method to display the person's details
    public void display() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

public class ClassesAndObjects {
    public static void main(String[] args) {
        // Creating objects
        Person person1 = new Person("Alice", 30);
        Person person2 = new Person("Bob", 25);

        // Calling methods on objects
        person1.display();
        person2.display();
    }
}

```

### Explanation:

1. **class Person**: Defines a class named `Person`.
2. **String name; int age;**: Declares instance variables for the class.
3. **public Person(String name, int age)**: A constructor to initialize the instance variables.
4. **public void display()**: A method to display the person's details.
5. **Person person1 = new Person("Alice", 30);**: Creates an object of the `Person` class.
6. **person1.display();**: Calls the `display` method on the `person1` object.

### Exercise 7:

1. Create a new file named `ClassesAndObjects.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try creating more objects and calling methods on them.

### Lesson 8: Inheritance

Inheritance allows a class to inherit fields and methods from another class. This promotes code reusability.

```java
javaCopy code
class Animal {
    public void eat() {
        System.out.println("This animal eats food.");
    }
}

class Dog extends Animal {
    public void bark() {
        System.out.println("The dog barks.");
    }
}

public class InheritanceExample {
    public static void main(String[] args) {
        Dog myDog = new Dog();
        myDog.eat();  // Inherited method
        myDog.bark(); // Method from Dog class
    }
}

```

### Explanation:

1. **class Animal**: A base class with a method `eat`.
2. **class Dog extends Animal**: A derived class that inherits from `Animal` and adds a new method `bark`.
3. **Dog myDog = new Dog();**: Creates an object of the `Dog` class.
4. **myDog.eat();**: Calls the inherited `eat` method.
5. **myDog.bark();**: Calls the `bark` method of the `Dog` class.

### Exercise 8:

1. Create a new file named `InheritanceExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try creating more classes and using inheritance to add functionality.

### Lesson 9: Interfaces

An interface is a reference type in Java, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types. Interfaces cannot contain instance fields or constructors.

```java
javaCopy code
interface Animal {
    void eat();
    void makeSound();
}

class Dog implements Animal {
    @Override
    public void eat() {
        System.out.println("The dog eats bones.");
    }

    @Override
    public void makeSound() {
        System.out.println("The dog barks.");
    }
}

public class InterfaceExample {
    public static void main(String[] args) {
        Dog myDog = new Dog();
        myDog.eat();
        myDog.makeSound();
    }
}

```

### Explanation:

1. **interface Animal**: Declares an interface named `Animal` with two abstract methods.
2. **class Dog implements Animal**: The `Dog` class implements the `Animal` interface and provides implementations for the `eat` and `makeSound` methods.
3. **myDog.eat();**: Calls the `eat` method on the `myDog` object.
4. **myDog.makeSound();**: Calls the `makeSound` method on the `myDog` object.

### Exercise 9:

1. Create a new file named `InterfaceExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try creating more classes that implement the `Animal` interface.

### Lesson 10: Abstract Classes

An abstract class cannot be instantiated and may contain abstract methods, which must be implemented by subclasses.

```java
abstract class Animal {
    abstract void eat();
    abstract void makeSound();
}

class Dog extends Animal {
    @Override
    public void eat() {
        System.out.println("The dog eats bones.");
    }

    @Override
    public void makeSound() {
        System.out.println("The dog barks.");
    }
}

public class AbstractClassExample {
    public static void main(String[] args) {
        Dog myDog = new Dog();
        myDog.eat();
        myDog.makeSound();
    }
}

```

### Explanation:

1. **abstract class Animal**: Declares an abstract class named `Animal` with two abstract methods.
2. **class Dog extends Animal**: The `Dog` class extends the `Animal` class and provides implementations for the `eat` and `makeSound` methods.
3. **Dog myDog = new Dog();**: Creates an object of the `Dog` class.
4. **myDog.eat();**: Calls the `eat` method on the `myDog` object.
5. **myDog.makeSound();**: Calls the `makeSound` method on the `myDog` object.

### Exercise 10:

1. Create a new file named `AbstractClassExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try creating more classes that extend the `Animal` abstract class.

### Lesson 11: Exception Handling

Exception handling in Java is managed via `try`, `catch`, `finally`, and `throw` keywords. It allows you to handle runtime errors, ensuring the normal flow of the program.

```java
javaCopy code
public class ExceptionHandlingExample {
    public static void main(String[] args) {
        try {
            int division = divide(10, 0);
            System.out.println("Result: " + division);
        } catch (ArithmeticException e) {
            System.out.println("Error: Cannot divide by zero.");
        } finally {
            System.out.println("This block always executes.");
        }
    }

    public static int divide(int a, int b) throws ArithmeticException {
        return a / b;
    }
}

```

### Explanation:

1. **try**: The block of code to be tested for errors.
2. **catch**: The block of code to be executed if an error occurs in the `try` block.
3. **finally**: The block of code that always executes, regardless of whether an exception is thrown or not.
4. **throws ArithmeticException**: Declares that the `divide` method may throw an `ArithmeticException`.

### Exercise 11:

1. Create a new file named `ExceptionHandlingExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try modifying the values to see different outcomes.

### Lesson 12: File I/O

Reading from and writing to files is a common task. Java provides several classes for file operations.

### Writing to a File

```java
javaCopy code
import java.io.FileWriter;
import java.io.IOException;

public class WriteToFileExample {
    public static void main(String[] args) {
        try {
            FileWriter writer = new FileWriter("output.txt");
            writer.write("Hello, world!");
            writer.close();
            System.out.println("Successfully wrote to the file.");
        } catch (IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}

```

### Explanation:

1. **FileWriter writer = new FileWriter("output.txt");**: Creates a `FileWriter` object to write to a file named `output.txt`.
2. **writer.write("Hello, world!");**: Writes the string to the file.
3. **writer.close();**: Closes the file writer.

### Exercise 12.1:

1. Create a new file named `WriteToFileExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Check the directory for the `output.txt` file to see the written content.

### Reading from a File

```java
javaCopy code
import java.io.File;
import java.io.FileNotFoundException;
import java.util.Scanner;

public class ReadFromFileExample {
    public static void main(String[] args) {
        try {
            File file = new File("output.txt");
            Scanner reader = new Scanner(file);
            while (reader.hasNextLine()) {
                String data = reader.nextLine();
                System.out.println(data);
            }
            reader.close();
        } catch (FileNotFoundException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}

```

### Explanation:

1. **File file = new File("output.txt");**: Creates a `File` object for the file named `output.txt`.
2. **Scanner reader = new Scanner(file);**: Creates a `Scanner` object to read from the file.
3. **reader.hasNextLine()**: Checks if the file has another line to read.
4. **String data = reader.nextLine();**: Reads the next line from the file.

### Exercise 12.2:

1. Create a new file named `ReadFromFileExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Ensure `output.txt` exists in the same directory with some content to read.

### Lesson 13: Collections

The Java Collections Framework provides a set of classes and interfaces to store and manipulate groups of data as a single unit. Let's look at some commonly used collections: `ArrayList`, `HashMap`, and `HashSet`.

### ArrayList

An `ArrayList` is a resizable array that can contain elements of a specific type.

```java
javaCopy code
import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        ArrayList<String> list = new ArrayList<>();

        // Adding elements to the ArrayList
        list.add("Apple");
        list.add("Banana");
        list.add("Orange");

        // Accessing elements
        System.out.println("First element: " + list.get(0));

        // Removing an element
        list.remove(1);

        // Iterating through the ArrayList
        System.out.println("Elements in the list:");
        for (String fruit : list) {
            System.out.println(fruit);
        }
    }
}

```

### Exercise 13.1:

1. Create a new file named `ArrayListExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try adding more elements, removing elements, and iterating in different ways.

### HashMap

A `HashMap` is a collection that stores key-value pairs. It allows you to map keys to values.

```java
javaCopy code
import java.util.HashMap;

public class HashMapExample {
    public static void main(String[] args) {
        HashMap<String, Integer> map = new HashMap<>();

        // Adding key-value pairs to the HashMap
        map.put("Apple", 1);
        map.put("Banana", 2);
        map.put("Orange", 3);

        // Accessing a value by key
        System.out.println("Value for 'Apple': " + map.get("Apple"));

        // Removing a key-value pair
        map.remove("Banana");

        // Iterating through the HashMap
        System.out.println("Elements in the map:");
        for (String key : map.keySet()) {
            System.out.println("Key: " + key + ", Value: " + map.get(key));
        }
    }
}

```

### Exercise 13.2:

1. Create a new file named `HashMapExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try adding more key-value pairs, removing pairs, and iterating in different ways.

### HashSet

A `HashSet` is a collection that contains no duplicate elements. It's useful for storing unique elements.

```java
javaCopy code
import java.util.HashSet;

public class HashSetExample {
    public static void main(String[] args) {
        HashSet<String> set = new HashSet<>();

        // Adding elements to the HashSet
        set.add("Apple");
        set.add("Banana");
        set.add("Orange");
        set.add("Apple");  // Duplicate element

        // Iterating through the HashSet
        System.out.println("Elements in the set:");
        for (String fruit : set) {
            System.out.println(fruit);
        }
    }
}

```

### Exercise 13.3:

1. Create a new file named `HashSetExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try adding more elements and observing how duplicates are handled.

### Lesson 14: Generics

Generics allow you to write flexible, reusable code by parameterizing types. Let's look at a simple example of a generic class.

```java
javaCopy code
public class GenericBox<T> {
    private T content;

    public void setContent(T content) {
        this.content = content;
    }

    public T getContent() {
        return content;
    }

    public static void main(String[] args) {
        GenericBox<String> stringBox = new GenericBox<>();
        stringBox.setContent("Hello, Generics!");
        System.out.println("String content: " + stringBox.getContent());

        GenericBox<Integer> integerBox = new GenericBox<>();
        integerBox.setContent(123);
        System.out.println("Integer content: " + integerBox.getContent());
    }
}

```

### Explanation:

1. **GenericBox<T>**: Declares a generic class with a type parameter `T`.
2. **setContent(T content)**: Sets the content of the box.
3. **getContent()**: Returns the content of the box.
4. **GenericBox<String> stringBox = new GenericBox<>();**: Creates a `GenericBox` object for `String` type.
5. **GenericBox<Integer> integerBox = new GenericBox<>();**: Creates a `GenericBox` object for `Integer` type.

### Exercise 14:

1. Create a new file named `GenericBox.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try creating more `GenericBox` objects with different types.

### Lesson 15: Multi-threading

Multi-threading allows you to perform multiple operations simultaneously. Let's look at creating and running threads in Java.

```java
javaCopy code
public class MultiThreadExample extends Thread {
    public void run() {
        for (int i = 1; i <= 5; i++) {
            System.out.println(Thread.currentThread().getId() + " Value: " + i);
            try {
                Thread.sleep(500); // Sleep for 500 milliseconds
            } catch (InterruptedException e) {
                System.out.println(e);
            }
        }
    }

    public static void main(String[] args) {
        MultiThreadExample thread1 = new MultiThreadExample();
        MultiThreadExample thread2 = new MultiThreadExample();

        thread1.start();
        thread2.start();
    }
}

```

### Explanation:

1. **extends Thread**: The `MultiThreadExample` class extends the `Thread` class.
2. **run()**: The `run` method contains the code that will be executed by the thread.
3. **thread1.start();**: Starts the first thread.
4. **thread2.start();**: Starts the second thread.

### Exercise 15:

1. Create a new file named `MultiThreadExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try creating more threads and observing how they run concurrently.

### Lesson 16: Advanced Exception Handling

Let's look at more advanced exception handling, including creating custom exceptions.

### Custom Exception

```java
javaCopy code
class CustomException extends Exception {
    public CustomException(String message) {
        super(message);
    }
}

public class CustomExceptionExample {
    public static void main(String[] args) {
        try {
            validateAge(15);
        } catch (CustomException e) {
            System.out.println("Caught the exception");
            System.out.println(e.getMessage());
        }
    }

    static void validateAge(int age) throws CustomException {
        if (age < 18) {
            throw new CustomException("Age must be 18 or above");
        } else {
            System.out.println("Valid age");
        }
    }
}

```

### Explanation:

1. **class CustomException extends Exception**: Declares a custom exception class.
2. **validateAge(int age) throws CustomException**: A method that throws a custom exception if the age is less than 18.
3. **throw new CustomException("Age must be 18 or above");**: Throws a custom exception with a message.

### Exercise 16:

1. Create a new file named `CustomExceptionExample.java`.
2. Copy the above code into this file.
3. Compile and run the program to see the output.
4. Try modifying the age to see different outcomes.

## Practice Programs

### Lesson 1: Basic Structure

1. Write a Java program that prints your name, age, and favorite hobby to the console.

### Lesson 2: Variables and Data Types

1. Create a program that declares variables of different data types (int, double, boolean, char, String) and prints their values.

### Lesson 3: Basic Operations

1. Write a program that takes two numbers as input and performs addition, subtraction, multiplication, and division. Print the results.

### Lesson 4: Control Structures

1. Create a program that checks if a number is positive, negative, or zero using an `if-else` statement.
2. Write a program that takes a score as input and prints the corresponding grade (A, B, C, D, F) using an `if-else` ladder.

### Lesson 5: Loops

1. Write a program that prints the numbers from 1 to 100 using a `for` loop.
2. Create a program that prints the even numbers between 1 and 50 using a `while` loop.

### Lesson 6: Methods

1. Write a program with a method that takes two integers as parameters and returns their sum. Call this method from the `main` method and print the result.
2. Create a method that checks if a given string is a palindrome.

### Lesson 7: Classes and Objects

1. Define a `Person` class with fields for name, age, and address. Create an object of this class and print its details.
2. Create a `Car` class with methods for starting, stopping, and displaying the car's details. Instantiate an object of this class and call its methods.

### Lesson 8: Inheritance

1. Create a base class `Animal` with a method `makeSound()`. Create derived classes `Dog` and `Cat` that override `makeSound()`. Test the classes by creating objects and calling their methods.

### Lesson 9: Interfaces

1. Define an interface `Shape` with methods `calculateArea()` and `calculatePerimeter()`. Implement this interface in classes `Circle` and `Rectangle`. Create objects of these classes and call their methods.

### Lesson 10: Abstract Classes

1. Create an abstract class `BankAccount` with methods `deposit()` and `withdraw()`. Extend this class in `SavingsAccount` and `CurrentAccount` classes. Implement the methods and test the classes.

### Lesson 11: Exception Handling

1. Write a program that handles an `ArrayIndexOutOfBoundsException` and prints an appropriate message.
2. Create a method that throws a custom exception `InsufficientFundsException` when a withdrawal amount exceeds the account balance.

### Lesson 12: File I/O

1. Write a program to write "Hello, world!" to a file named `hello.txt`.
2. Create a program that reads from a file named `data.txt` and prints its contents to the console.

### Lesson 13: Collections

1. Write a program that uses an `ArrayList` to store and print a list of fruits.
2. Create a program that uses a `HashMap` to store and print student names and their corresponding grades.
3. Write a program that uses a `HashSet` to store and print unique cities.

### Lesson 14: Generics

1. Create a generic class `Box` that can store objects of any type. Test this class with different data types.
2. Write a generic method that takes an array of any type and prints its elements.

### Lesson 15: Multi-threading

1. Write a program that creates two threads. Each thread should print numbers from 1 to 5, pausing for 1 second between each number.
2. Create a program where two threads share a common resource (e.g., a counter). Ensure that the resource is accessed safely using synchronization.

### Lesson 16: Advanced Exception Handling

1. Create a custom exception `InvalidAgeException` and write a program that throws this exception if an invalid age (negative or over 150) is entered.
2. Write a program that demonstrates the use of multiple catch blocks for different exception types.

### Bonus: Combining Concepts

1. Write a complete program that includes reading data from a file, processing it using collections, and handling any exceptions that may occur.
2. Create a mini-banking application with classes for accounts, transactions, and customers. Include features like deposit, withdrawal, and balance inquiry. Use exception handling for error scenarios and collections to manage multiple accounts.

## Answers

### Lesson 1: Basic Structure

1. **Print name, age, and favorite hobby:**

```java
javaCopy code
public class PrintDetails {
    public static void main(String[] args) {
        System.out.println("Name: John Doe");
        System.out.println("Age: 25");
        System.out.println("Favorite Hobby: Reading");
    }
}

```

### Lesson 2: Variables and Data Types

1. **Declare and print variables of different data types:**

```java
javaCopy code
public class DataTypesExample {
    public static void main(String[] args) {
        int age = 25;
        double height = 5.9;
        boolean isStudent = true;
        char grade = 'A';
        String name = "John Doe";

        System.out.println("Age: " + age);
        System.out.println("Height: " + height);
        System.out.println("Is Student: " + isStudent);
        System.out.println("Grade: " + grade);
        System.out.println("Name: " + name);
    }
}

```

### Lesson 3: Basic Operations

1. **Perform basic arithmetic operations:**

```java
javaCopy code
import java.util.Scanner;

public class BasicOperations {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter first number: ");
        double num1 = scanner.nextDouble();

        System.out.print("Enter second number: ");
        double num2 = scanner.nextDouble();

        System.out.println("Sum: " + (num1 + num2));
        System.out.println("Difference: " + (num1 - num2));
        System.out.println("Product: " + (num1 * num2));
        System.out.println("Quotient: " + (num1 / num2));
    }
}

```

### Lesson 4: Control Structures

1. **Check if a number is positive, negative, or zero:**

```java
javaCopy code
import java.util.Scanner;

public class CheckNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int number = scanner.nextInt();

        if (number > 0) {
            System.out.println("The number is positive.");
        } else if (number < 0) {
            System.out.println("The number is negative.");
        } else {
            System.out.println("The number is zero.");
        }
    }
}

```

1. **Print grade based on score:**

```java
javaCopy code
import java.util.Scanner;

public class GradeCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter your score: ");
        int score = scanner.nextInt();

        if (score >= 90) {
            System.out.println("Grade: A");
        } else if (score >= 80) {
            System.out.println("Grade: B");
        } else if (score >= 70) {
            System.out.println("Grade: C");
        } else if (score >= 60) {
            System.out.println("Grade: D");
        } else {
            System.out.println("Grade: F");
        }
    }
}

```

### Lesson 5: Loops

1. **Print numbers from 1 to 100 using a `for` loop:**

```java
javaCopy code
public class ForLoopExample {
    public static void main(String[] args) {
        for (int i = 1; i <= 100; i++) {
            System.out.println(i);
        }
    }
}

```

1. **Print even numbers between 1 and 50 using a `while` loop:**

```java
javaCopy code
public class WhileLoopExample {
    public static void main(String[] args) {
        int i = 1;

        while (i <= 50) {
            if (i % 2 == 0) {
                System.out.println(i);
            }
            i++;
        }
    }
}

```

### Lesson 6: Methods

1. **Method to sum two integers:**

```java
javaCopy code
public class SumMethod {
    public static int sum(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int result = sum(10, 20);
        System.out.println("Sum: " + result);
    }
}

```

1. **Method to check if a string is a palindrome:**

```java
javaCopy code
public class PalindromeCheck {
    public static boolean isPalindrome(String str) {
        int left = 0;
        int right = str.length() - 1;

        while (left < right) {
            if (str.charAt(left) != str.charAt(right)) {
                return false;
            }
            left++;
            right--;
        }

        return true;
    }

    public static void main(String[] args) {
        String word = "radar";
        System.out.println(word + " is a palindrome: " + isPalindrome(word));
    }
}

```

### Lesson 7: Classes and Objects

1. **Person class:**

```java
javaCopy code
class Person {
    String name;
    int age;
    String address;

    Person(String name, int age, String address) {
        this.name = name;
        this.age = age;
        this.address = address;
    }

    void displayDetails() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Address: " + address);
    }
}

public class PersonExample {
    public static void main(String[] args) {
        Person person = new Person("John Doe", 25, "123 Main St");
        person.displayDetails();
    }
}

```

1. **Car class:**

```java
javaCopy code
class Car {
    String make;
    String model;
    int year;

    Car(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    void start() {
        System.out.println("The car is starting.");
    }

    void stop() {
        System.out.println("The car is stopping.");
    }

    void displayDetails() {
        System.out.println("Make: " + make);
        System.out.println("Model: " + model);
        System.out.println("Year: " + year);
    }
}

public class CarExample {
    public static void main(String[] args) {
        Car car = new Car("Toyota", "Camry", 2020);
        car.start();
        car.displayDetails();
        car.stop();
    }
}

```

### Lesson 8: Inheritance

1. **Animal inheritance example:**

```java
javaCopy code
class Animal {
    void makeSound() {
        System.out.println("Animal sound");
    }
}

class Dog extends Animal {
    @Override
    void makeSound() {
        System.out.println("Bark");
    }
}

class Cat extends Animal {
    @Override
    void makeSound() {
        System.out.println("Meow");
    }
}

public class InheritanceExample {
    public static void main(String[] args) {
        Dog dog = new Dog();
        Cat cat = new Cat();

        dog.makeSound();
        cat.makeSound();
    }
}

```

### Lesson 9: Interfaces

1. **Shape interface example:**

```java
javaCopy code
interface Shape {
    double calculateArea();
    double calculatePerimeter();
}

class Circle implements Shape {
    private double radius;

    Circle(double radius) {
        this.radius = radius;
    }

    @Override
    public double calculateArea() {
        return Math.PI * radius * radius;
    }

    @Override
    public double calculatePerimeter() {
        return 2 * Math.PI * radius;
    }
}

class Rectangle implements Shape {
    private double length;
    private double width;

    Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    @Override
    public double calculateArea() {
        return length * width;
    }

    @Override
    public double calculatePerimeter() {
        return 2 * (length + width);
    }
}

public class InterfaceExample {
    public static void main(String[] args) {
        Circle circle = new Circle(5);
        Rectangle rectangle = new Rectangle(4, 6);

        System.out.println("Circle Area: " + circle.calculateArea());
        System.out.println("Circle Perimeter: " + circle.calculatePerimeter());
        System.out.println("Rectangle Area: " + rectangle.calculateArea());
        System.out.println("Rectangle Perimeter: " + rectangle.calculatePerimeter());
    }
}

```

### Lesson 10: Abstract Classes

1. **BankAccount abstract class example:**

```java
javaCopy code
abstract class BankAccount {
    double balance;

    BankAccount(double balance) {
        this.balance = balance;
    }

    abstract void deposit(double amount);
    abstract void withdraw(double amount);
}

class SavingsAccount extends BankAccount {
    SavingsAccount(double balance) {
        super(balance);
    }

    @Override
    void deposit(double amount) {
        balance += amount;
        System.out.println("Deposited: " + amount + ", New Balance: " + balance);
    }

    @Override
    void withdraw(double amount) {
        if (amount <= balance) {
            balance -= amount;
            System.out.println("Withdrew: " + amount + ", New Balance: " + balance);
        } else {
            System.out.println("Insufficient funds");
        }
    }
}

class CurrentAccount extends BankAccount {
    CurrentAccount(double balance) {
        super(balance);
    }

    @Override
    void deposit(double amount) {
        balance += amount;
        System.out.println("Deposited: " + amount + ", New Balance: " + balance);
    }

    @Override
    void withdraw(double amount) {
        if (amount <= balance) {
            balance -= amount;
            System.out.println("Withdrew: " + amount + ", New Balance: " + balance);
        } else {
            System.out.println("Insufficient funds");
        }
    }
}

public class AbstractClassExample {
    public static void main(String[] args) {
        SavingsAccount savingsAccount = new SavingsAccount(1000);
        savingsAccount.deposit(200);
        savingsAccount.withdraw(500);

        CurrentAccount currentAccount = new CurrentAccount(2000);
        currentAccount.deposit(500);
        currentAccount.withdraw(1000);
    }
}

```

### Lesson 11: Exception Handling

1. **Handle `ArrayIndexOutOfBoundsException`:**

```java
javaCopy code
public class ArrayExceptionHandling {
    public static void main(String[] args) {
        int[] array = {1, 2, 3};

        try {
            System.out.println(array[3]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Array index is out of bounds");
        }
    }
}

```

1. **Custom exception `InsufficientFundsException`:**

```java
javaCopy code
class InsufficientFundsException extends Exception {
    InsufficientFundsException(String message) {
        super(message);
    }
}

class BankAccount {
    private double balance;

    BankAccount(double balance) {
        this.balance = balance;
    }

    void withdraw(double amount) throws InsufficientFundsException {
        if (amount > balance) {
            throw new InsufficientFundsException("Insufficient funds for withdrawal");
        } else {
            balance -= amount;
            System.out.println("Withdrawn: " + amount + ", New Balance: " + balance);
        }
    }
}

public class CustomExceptionExample {
    public static void main(String[] args) {
        BankAccount account = new BankAccount(500);

        try {
            account.withdraw(600);
        } catch (InsufficientFundsException e) {
            System.out.println(e.getMessage());
        }
    }
}

```

### Lesson 12: File I/O

1. **Write to a file:**

```java
javaCopy code
import java.io.FileWriter;
import java.io.IOException;

public class WriteToFile {
    public static void main(String[] args) {
        try {
            FileWriter writer = new FileWriter("hello.txt");
            writer.write("Hello, world!");
            writer.close();
            System.out.println("Successfully wrote to the file.");
        } catch (IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}

```

1. **Read from a file:**

```java
javaCopy code
import java.io.File;
import java.io.FileNotFoundException;
import java.util.Scanner;

public class ReadFromFile {
    public static void main(String[] args) {
        try {
            File file = new File("data.txt");
            Scanner scanner = new Scanner(file);

            while (scanner.hasNextLine()) {
                String data = scanner.nextLine();
                System.out.println(data);
            }
            scanner.close();
        } catch (FileNotFoundException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
        }
    }
}

```

### Lesson 13: Collections

1. **ArrayList of fruits:**

```java
javaCopy code
import java.util.ArrayList;

public class FruitList {
    public static void main(String[] args) {
        ArrayList<String> fruits = new ArrayList<>();
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Orange");

        for (String fruit : fruits) {
            System.out.println(fruit);
        }
    }
}

```

1. **HashMap of students and grades:**

```java
javaCopy code
import java.util.HashMap;
import java.util.Map;

public class StudentGrades {
    public static void main(String[] args) {
        HashMap<String, String> grades = new HashMap<>();
        grades.put("John", "A");
        grades.put("Jane", "B");
        grades.put("Jack", "C");

        for (Map.Entry<String, String> entry : grades.entrySet()) {
            System.out.println("Student: " + entry.getKey() + ", Grade: " + entry.getValue());
        }
    }
}

```

1. **HashSet of unique cities:**

```java
javaCopy code
import java.util.HashSet;

public class UniqueCities {
    public static void main(String[] args) {
        HashSet<String> cities = new HashSet<>();
        cities.add("New York");
        cities.add("Los Angeles");
        cities.add("Chicago");
        cities.add("New York"); // Duplicate entry

        for (String city : cities) {
            System.out.println(city);
        }
    }
}

```

### Lesson 14: Generics

1. **Generic `Box` class:**

```java
javaCopy code
class Box<T> {
    private T value;

    Box(T value) {
        this.value = value;
    }

    T getValue() {
        return value;
    }

    void setValue(T value) {
        this.value = value;
    }
}

public class GenericBoxExample {
    public static void main(String[] args) {
        Box<Integer> intBox = new Box<>(123);
        System.out.println("Integer value: " + intBox.getValue());

        Box<String> strBox = new Box<>("Hello");
        System.out.println("String value: " + strBox.getValue());
    }
}

```

1. **Generic method to print array elements:**

```java
javaCopy code
public class GenericMethodExample {
    public static <T> void printArray(T[] array) {
        for (T element : array) {
            System.out.println(element);
        }
    }

    public static void main(String[] args) {
        Integer[] intArray = {1, 2, 3, 4, 5};
        String[] strArray = {"A", "B", "C", "D", "E"};

        System.out.println("Integer array:");
        printArray(intArray);

        System.out.println("String array:");
        printArray(strArray);
    }
}

```

### Lesson 15: Multi-threading

1. **Two threads printing numbers:**

```java
javaCopy code
class NumberThread extends Thread {
    private String threadName;

    NumberThread(String threadName) {
        this.threadName = threadName;
    }

    public void run() {
        try {
            for (int i = 1; i <= 5; i++) {
                System.out.println(threadName + ": " + i);
                Thread.sleep(1000);
            }
        } catch (InterruptedException e) {
            System.out.println(threadName + " interrupted.");
        }
    }
}

public class MultiThreadExample {
    public static void main(String[] args) {
        NumberThread thread1 = new NumberThread("Thread 1");
        NumberThread thread2 = new NumberThread("Thread 2");

        thread1.start();
        thread2.start();
    }
}

```

1. **Threads sharing a common resource:**

```java
javaCopy code
class Counter {
    private int count = 0;

    public synchronized void increment() {
        count++;
    }

    public int getCount() {
        return count;
    }
}

class CounterThread extends Thread {
    private Counter counter;

    CounterThread(Counter counter) {
        this.counter = counter;
    }

    public void run() {
        for (int i = 0; i < 1000; i++) {
            counter.increment();
        }
    }
}

public class SynchronizedExample {
    public static void main(String[] args) {
        Counter counter = new Counter();
        CounterThread thread1 = new CounterThread(counter);
        CounterThread thread2 = new CounterThread(counter);

        thread1.start();
        thread2.start();

        try {
            thread1.join();
            thread2.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        System.out.println("Final count: " + counter.getCount());
    }
}

```

### Lesson 16: Advanced Exception Handling

1. **Custom exception `InvalidAgeException`:**

```java
javaCopy code
class InvalidAgeException extends Exception {
    InvalidAgeException(String message) {
        super(message);
    }
}

public class AgeCheck {
    public static void checkAge(int age) throws InvalidAgeException {
        if (age < 0 || age > 150) {
            throw new InvalidAgeException("Invalid age: " + age);
        } else {
            System.out.println("Valid age: " + age);
        }
    }

    public static void main(String[] args) {
        try {
            checkAge(200);
        } catch (InvalidAgeException e) {
            System.out.println(e.getMessage());
        }
    }
}

```

1. **Multiple catch blocks:**

```java
javaCopy code
public class MultipleCatchExample {
    public static void main(String[] args) {
        try {
            int[] array = new int[5];
            array[10] = 30 / 0;
        } catch (ArithmeticException e) {
            System.out.println("ArithmeticException: " + e.getMessage());
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("ArrayIndexOutOfBoundsException: " + e.getMessage());
        } catch (Exception e) {
            System.out.println("Exception: " + e.getMessage());
        }
    }
}

```