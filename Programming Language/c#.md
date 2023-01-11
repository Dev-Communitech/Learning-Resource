# C# (pronounced "C-sharp")

C# (pronounced "C-sharp") is a modern, object-oriented programming language developed by Microsoft. It is designed to be simple, safe, and powerful, and it is commonly used to build Windows desktop applications, Windows Store apps, web applications, and games. C# is part of the .NET ecosystem, which also includes the .NET Framework, an extensive library of pre-written code, and the Common Language Runtime (CLR), which manages the execution of .NET programs.

C# syntax is heavily influenced by C and C++, but it also incorporates elements from other languages such as Java and Delphi. C# supports features such as strong type checking, automatic memory management, and garbage collection. It also includes support for modern programming constructs like lambda expressions, generics, and async/await.

# Here is an example of a "Hello, World!" program written in C#:
```
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, World!");
    }
}
```
This program defines a Main method that is the entry point of every C# program. The Console.WriteLine method is used to print a string to the console. The using directive is used to include the System namespace, which contains the Console class.

# A simple command-line calculator that can perform addition, subtraction, multiplication, and division:
```
using System;

class Calculator
{
    static void Main()
    {
        double num1, num2;
        char operation;

        Console.WriteLine("Simple Calculator");
        Console.WriteLine("Enter first number:");
        num1 = double.Parse(Console.ReadLine());

        Console.WriteLine("Enter operation (+, -, *, /):");
        operation = char.Parse(Console.ReadLine());

        Console.WriteLine("Enter second number:");
        num2 = double.Parse(Console.ReadLine());

        switch (operation)
        {
            case '+':
                Console.WriteLine($"{num1} + {num2} = {num1 + num2}");
                break;
            case '-':
                Console.WriteLine($"{num1} - {num2} = {num1 - num2}");
                break;
            case '*':
                Console.WriteLine($"{num1} * {num2} = {num1 * num2}");
                break;
            case '/':
                Console.WriteLine($"{num1} / {num2} = {num1 / num2}");
                break;
            default:
                Console.WriteLine("Invalid operation");
                break;
        }
    }
}
```
# A simple web server using the ASP.NET Core framework:
```
using Microsoft.AspNetCore.Builder;
using Microsoft.AspNetCore.Hosting;
using Microsoft.AspNetCore.Http;

class Program
{
    public static void Main(string[] args)
    {
        var host = new WebHostBuilder()
            .UseKestrel()
            .Configure(app => app.Run(context => context.Response.WriteAsync("Hello, World!")))
            .Build();

        host.Run();
    }
}
```
You can build this program by using IDE such as Visual Studio, or by using the command line interface and the command csc which is the C# compiler, this will produce an executable file from your source code, then you can run the resulting file.

C# is widely adopted and it's used for a wide range of purpose and platforms, from Windows, Web, mobile, games, and more. It's a mature and stable language with a large community, variety of libraries and frameworks which help developers building their software with ease.

