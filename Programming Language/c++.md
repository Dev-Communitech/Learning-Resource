# C++ 

C++ is a high-level, general-purpose programming language that was developed by Bjarne Stroustrup in 1979 as an extension of the C programming language. It is an object-oriented language, which means that it allows programmers to define data types in the form of classes and objects.

One of the main features of C++ is its support for object-oriented programming, which allows programmers to define classes that represent real-world objects and the functions that operate on them. This helps to make C++ code more modular and easier to maintain, as it allows developers to create reusable blocks of code that can be easily modified and extended.

C++ is also a statically-typed language, which means that variables must be declared with a specific type before they can be used in a program. This helps to prevent errors by ensuring that the type of a variable is known at compile-time, rather than at runtime.

In addition to its object-oriented and statically-typed features, C++ also has a number of other features that make it a popular choice for a wide range of programming tasks. These include support for procedural programming, a rich standard library, and low-level control over system resources.

C++ is widely used in a variety of contexts, including operating systems, web browsers, games, and scientific applications. It is also the primary language used in the development of the Linux kernel, and is commonly used in the development of other open-source software projects.

# A Simple C++ Program That Prompts The User To Enter Their Name And Then Prints It to The Screen:

```c++
#include <iostream>
#include <string>

int main() {
  std::string name;

  std::cout << "Enter your name: ";
  std::cin >> name;

  std::cout << "Hello, " << name << "!" << std::endl;

  return 0;
}
```
This program includes two headers, iostream and string. The iostream header provides input and output stream objects, such as cin and cout, which are used to read from and write to the standard input and output streams, respectively. The string header provides the string class, which is used to store and manipulate string data.

The main function is the entry point of the program. It begins by declaring a variable of type string called name. The cout object is then used to output a prompt to the user asking them to enter their name. The cin object is then used to read the user's input and store it in the name variable. Finally, the program outputs a greeting to the user using the cout object and the name variable.

# A program that calculates the area and perimeter of a rectangle:

```c++
#include <iostream>

int main() {
  double width, height;

  std::cout << "Enter the width of the rectangle: ";
  std::cin >> width;

  std::cout << "Enter the height of the rectangle: ";
  std::cin >> height;

  double area = width * height;
  double perimeter = 2 * (width + height);

  std::cout << "The area of the rectangle is: " << area << std::endl;
  std::cout << "The perimeter of the rectangle is: " << perimeter << std::endl;

  return 0;
}
```

```
