# Java Hello World Project

A basic Java program that demonstrates the fundamentals of Java syntax and the compilation process.

## 📁 Project Structure
```
hello-world/
├── README.md           # This file
├── src/                # Source code directory
│   └── MyFirstProgram.java
├── classes/            # Compiled bytecode directory
└── test/              # Test files directory
```

## 💻 Program Code

**File:** `src/MyFirstProgram.java`

```java
public class MyFirstProgram {
    public static void main(String s[]) {
        System.out.println("Hello World!");
    }
}
```

## 📖 Line-by-Line Explanation

1. **`public class MyFirstProgram {`**
   - `public` - Access modifier making the class visible to other classes
   - `class` - Keyword declaring this is a class definition
   - `MyFirstProgram` - The class name (must match the filename)
   - `{` - Opens the class body

2. **`public static void main(String s[]) {`**
   - `public` - Access modifier allowing the method to be called from outside the class
   - `static` - Method belongs to the class itself, not to any instance
   - `void` - Return type indicating the method doesn't return any value
   - `main` - Special method name that serves as the program entry point
   - `String s[]` - Parameter accepting an array of command-line arguments
   - `{` - Opens the method body

3. **`System.out.println("Hello World!");`**
   - `System` - Built-in Java class containing system-related functionality
   - `out` - Static field of System class representing standard output stream
   - `println` - Method that prints text followed by a newline character
   - `"Hello World!"` - String literal to be printed
   - `;` - Statement terminator

4. **`}`** - Closes the main method body
5. **`}`** - Closes the class body

## ⚙️ Compilation and Execution

### Prerequisites
- Java Development Kit (JDK) installed
- Command line access

### To compile:
```bash
# Navigate to the project directory
cd languages/java/hello-world

# Compile the source code
javac -d classes src/MyFirstProgram.java
```

**Command breakdown:**
- `javac` - Java compiler
- `-d classes` - Specifies output directory for compiled bytecode
- `src/MyFirstProgram.java` - Path to the source file

### To run:
```bash
# Run the compiled program
java -cp classes MyFirstProgram
```

**Command breakdown:**
- `java` - Java runtime
- `-cp classes` - Sets classpath to the classes directory
- `MyFirstProgram` - Name of the class containing main method

### Expected Output:
```
Hello World!
```

## 🎯 What You'll Learn

- Understanding Java class structure
- The role of the main method as program entry point
- Basic output using System.out.println()
- Java compilation process (source code → bytecode)
- How to run Java programs from command line

## 🔗 Related Concepts

- **Java Virtual Machine (JVM)**: Executes Java bytecode
- **Platform Independence**: Compiled Java runs on any system with JVM
- **Object-Oriented Programming**: Classes are blueprints for objects
- **Static Methods**: Belong to class, not instances

## ➡️ Next Steps

Try modifying the program:
1. Change the output message
2. Add multiple println statements
3. Add comments to explain your code
4. Create additional methods within the class