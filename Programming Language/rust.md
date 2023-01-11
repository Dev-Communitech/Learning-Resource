# RUST

Rust is a programming language designed for safety, concurrency, and performance. It is a statically-typed language, meaning that you must specify the type of a variable when you declare it, and this type cannot change later. Rust also has a strong emphasis on ownership and borrowing, which helps prevent null or dangling pointer references and allows for safe concurrency.

Some notable features of Rust include:

Zero-cost abstractions: You can write high-level code that is just as performant as low-level code.

Ownership and borrowing: Rust's ownership system allows you to write code that is free of null or dangling pointer references. The borrowing system allows you to safely share and use data in a concurrent environment.

Safe concurrency: Rust's ownership and borrowing rules, combined with its support for lightweight threads, make it easy to write concurrent code that is both correct and performant.

High-level abstractions: Rust has a number of features that make it easier to write code at a high level of abstraction, such as iterators, closures, and pattern matching.

Compatibility with C: You can call C code from Rust and vice versa, making it easy to integrate Rust code into a larger system.

# Here is an example of a "Hello, World!" program written in Rust:
```
fn main() {
    println!("Hello, World!");
}
```
This program defines a main function, which is the entry point of every Rust program. The println! macro is used to print a string to the console. The ! after the name indicates that this is a macro, not a function. Macros in Rust are similar to functions, but they generate code at compile-time rather than being called at runtime.

# A simple command-line calculator that can perform addition, subtraction, multiplication, and division:
```
use std::io;

fn main() {
    let mut input = String::new();
    let mut num1: f64 = 0.0;
    let mut num2: f64 = 0.0;
    let mut operation: char = ' ';

    println!("Simple Calculator");
    println!("Enter first number:");
    io::stdin().read_line(&mut input).unwrap();
    num1 = input.trim().parse().unwrap();
    input.clear();

    println!("Enter operation (+, -, *, /):");
    io::stdin().read_line(&mut input).unwrap();
    operation = input.trim().parse().unwrap();
    input.clear();

    println!("Enter second number:");
    io::stdin().read_line(&mut input).unwrap();
    num2 = input.trim().parse().unwrap();
    input.clear();

    match operation {
        '+' => println!("{} + {} = {}", num1, num2, num1 + num2),
        '-' => println!("{} - {} = {}", num1, num2, num1 - num2),
        '*' => println!("{} * {} = {}", num1, num2, num1 * num2),
        '/' => println!("{} / {} = {}", num1, num2, num1 / num2),
        _   => println!("Invalid operation"),
    }
}
```

# A program that reads the contents of a text file and prints them to the console:
```
use std::fs::File;
use std::io::prelude::*;

fn main() {
    let mut file = File::open("example.txt").expect("Could not open file");
    let mut contents = String::new();
    file.read_to_string(&mut contents).expect("Could not read file");
    println!("{}", contents);
}
```

