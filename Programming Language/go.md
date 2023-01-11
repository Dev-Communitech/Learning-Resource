# GO_LANG

Go, also known as Golang, is a programming language developed by Google in 2009. It was designed to be a fast, statically-typed, compiled language that is easy to read and write, with efficient concurrency support.

One of the key features of Go is its support for concurrent programming. It has built-in primitives for creating and managing goroutines, which are lightweight threads of execution, and channels, which are used for communication between goroutines. This makes it easy to write programs that can perform multiple tasks concurrently and communicate with each other through channels.

Go is also known for its simplicity and clarity. It has a small and consistent standard library, and its syntax is clean and easy to read. It also has a number of built-in tools for debugging and testing, including the go test command, which allows developers to write and run unit tests.

In addition to its simplicity and concurrency support, Go is also known for its performance. It is a compiled language, which means that it is converted to machine code before it is executed, making it faster than many interpreted languages. It also has a number of optimization features, such as garbage collection and inlining, which can help improve the performance of Go programs.

Go has become popular in a variety of fields, including web development, system programming, and data analysis. It is used by companies such as Google, Uber, and Dropbox, and has a large and active community of users and contributors.

# Here's a simple "Hello, World!" program written in Go:
```
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```
This program defines a main function, which is the entry point of the program. Inside the function, it calls the Println function from the fmt package to print the string "Hello, World!" to the console.

# here is a more complex example in Go, which demonstrates some of the language's features:
```
package main

import (
    "fmt"
    "math"
)

type Circle struct {
    x, y, r float64
}

func (c *Circle) area() float64 {
    return math.Pi * c.r * c.r
}

func main() {
    c := Circle{x: 0, y: 0, r: 5}
    fmt.Println("Area of circle:", c.area())
}
```
This program defines a Circle struct that has three fields: x, y, and r, which represent the x and y coordinates of the center of the circle, and the radius of the circle, respectively. The program also defines a method named area for the Circle struct which calculates the area of the circle.

The main function then creates a Circle variable with the given x, y, and r values and calls the area method. Finally, it prints out the calculated area.

This program demonstrates some of the language's features such as struct, method, and calling external packages such as math package. 

#  here's another example in Go that demonstrates concurrency, one of the language's key features:
```
package main

import (
    "fmt"
    "time"
)

func printNumbers() {
    for i := 1; i <= 10; i++ {
        fmt.Print(i, " ")
        time.Sleep(time.Millisecond * 100)
    }
}

func printLetters() {
    for i := 'A'; i <= 'J'; i++ {
        fmt.Print(string(i), " ")
        time.Sleep(time.Millisecond * 100)
    }
}

func main() {
    go printNumbers()
    go printLetters()
    time.Sleep(time.Millisecond * 1110)
    fmt.Println("\nExiting...")
}
```
This program defines two functions: printNumbers and printLetters, each of which will print out numbers and letters respectively with a 100ms sleep time.

The main function starts both functions as goroutines using the go keyword and then waits for 1.1s before exiting. Because the two goroutines run concurrently, the numbers and letters will be printed in an interleaved fashion, with the exact output depending on the scheduling of the goroutines by the Go runtime.

This example demonstrates how easy it is to create concurrent program in Go and it utilizes the powerful inbuilt concurrency primitives such as goroutine and channel. Goroutines are lightweight threads of execution that can run concurrently with other goroutines. With goroutines, it's easy to create concurrent programs that can perform multiple tasks at the same time. Go also provides other primitives like channels that allow goroutines to communicate and synchronize with each other.
