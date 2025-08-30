# Java Hello World Program

### Project Structure
```
Java/helloWorld/
├── src/                 # Source code directory
├── classes/             # Compiled bytecode directory
└── test/                # Test files directory
```

### Program Code
Located at: `Java/helloWorld/src/MyFirstJavaProgram.java`

```java
public class MyFirstJavaProgram {
    public static void main(String s[]) {
        System.out.println("Hello World!");
    }
}
```

### Line-by-Line Explanation

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

### Compilation and Execution

#### To compile:
```bash
# Navigate to the project directory
cd Java/helloWorld

# Compile the source code
javac -d classes src/MyFirstJavaProgram.java
```

This command:
- `javac` - Java compiler
- `-d classes` - Specifies output directory for compiled bytecode
- `src/MyFirstProgram.java` - Path to the source file

#### To run:
```bash
# Run the compiled program
java -cp classes MyFirstJavaProgram
```

This command:
- `java` - Java runtime
- `-cp classes` - Sets classpath to the classes directory
- `MyFirstJavaProgram` - Name of the class containing main method

