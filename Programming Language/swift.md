# Swift
Swift is a programming language developed by Apple Inc. It is primarily used to develop applications for iOS, iPadOS, macOS, watchOS, and tvOS. 
Swift is a statically-typed language, meaning that you must specify the type of a variable when you declare it, and this type cannot change later.

# Here is a simple example of a Swift program that prints a message:
```
print("Hello, World!")
```
This program has a single line of code that uses the print function to print a string to the console.

# Here is an example of a Swift function:
```
func greet(name: String) -> String {
  return "Hello, \(name)!"
}
```
This function, called greet, takes a single argument called name of type String and returns a String. It uses string interpolation to build a greeting message and returns it.

 # Here is an example of how you might use this function in a Swift program:
 ```
 let greeting = greet(name: "Alice")
print(greeting) // Prints "Hello, Alice!"
```
This program calls the greet function and stores the result in a constant called greeting. It then prints the greeting to the console.
