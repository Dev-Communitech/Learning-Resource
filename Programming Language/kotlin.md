# Kotlin
Kotlin is a programming language developed by JetBrains. It is a statically-typed language that runs on the Java Virtual Machine (JVM) and can also be compiled to JavaScript or native code. Kotlin is fully interoperable with Java, meaning that you can use Kotlin code in a Java project and vice versa.

# Here is a simple example of a Kotlin program that prints a message :
```
fun main() {
  println("Hello, World!")
}
```
This program has a single function, main, which is the entry point of every Kotlin program. The main function contains a single line of code that uses the println function to print a string to the console.

# Here is an example of a Kotlin function:
```
fun greet(name: String): String {
  return "Hello, $name!"
}
```
This function, called greet, takes a single argument called name of type String and returns a String. It uses string template to build a greeting message and returns it.
# Here is an example of how you might use this function in a Kotlin program:
```
fun main() {
  val greeting = greet("Alice")
  println(greeting) // Prints "Hello, Alice!"
}
```
This program calls the greet function and stores the result in a variable called greeting. It then prints the greeting to the console.

# Here is an example of a Kotlin class:
```
class Person(val name: String, val age: Int) {
  fun greet() = "Hello, my name is $name and I am $age years old."
}
```
This class, called Person, represents a person with a name and an age. It has two properties, name and age, which represent the name and age of the person, respectively. It has a single method, greet, which returns a string that introduces the person.



