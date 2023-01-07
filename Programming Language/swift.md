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

# Here is an example of a Swift class:
```
class Person {
  var name: String
  var age: Int

  init(name: String, age: Int) {
    self.name = name
    self.age = age
  }

  func greet() -> String {
    return "Hello, my name is \(name) and I am \(age) years old."
  }
}
```
This class, called Person, represents a person with a name and an age. It has two fields, name and age, which represent the name and age of the person, respectively. It has a single initializer, which takes two arguments and initializes the name and age fields. It also has a single method, greet, which returns a string that introduces the person.

# Here is an example of how you might use this class in a Swift program:
```
let p = Person(name: "Alice", age: 30)
print(p.greet()) // Prints "Hello, my name is Alice and I am 30 years old."
```

