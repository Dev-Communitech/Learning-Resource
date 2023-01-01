# RUBY
Ruby is a popular programming language that is known for its simplicity, readability, and flexibility. It was created in the mid-1990s by Yukihiro "Matz" Matsumoto in Japan, and has since gained a large and active community of developers around the world.

One of the key features of Ruby is its use of code blocks, which are chunks of code that can be passed as arguments to methods. This allows developers to write concise, expressive code and makes it easy to write code that is easy to read and understand.

Ruby is also dynamically-typed, which means that you don't have to specify the data type of a variable when you declare it. This can make it easier to write code quickly, as you don't have to spend time thinking about the type of data that your variables will hold.

In addition to its simplicity and expressiveness, Ruby is also highly extensible. It has a large standard library and a wealth of third-party libraries, or "gems," that can be easily added to a Ruby project. This makes it easy to add new functionality to your code without having to reinvent the wheel.

Overall, Ruby is a great choice for developers who want to write clean, readable, and flexible code. It is used in a wide variety of projects, including web applications, data analysis, and automation scripts. So, it is a very useful programming language to learn and work with.

# BASIC PROGRAM IN RUBY

Write a program that prints the numbers from 1 to 100. For multiples of three, print "Fizz" instead of the number, and for multiples of five, print "Buzz". For numbers that are multiples of both three and five, print "FizzBuzz".

```for i in 1..100
  if i % 3 == 0 && i % 5 == 0
    puts "FizzBuzz"
  elsif i % 3 == 0
    puts "Fizz"
  elsif i % 5 == 0
    puts "Buzz"
  else
    puts i
  end
end
```
Write a program that calculates the factorial of a number. The factorial of a number is the product of all the integers from 1 to that number. For example, the factorial of 5 is 5 * 4 * 3 * 2 * 1 = 120.
```def factorial(n)
  if n <= 1
    1
  else
    n * factorial(n-1)
  end
end

puts factorial(5)  # Output: 120
```

Write a program that takes an array of integers and returns a new array with the elements in reverse order.
```def reverse_array(arr)
  reversed_arr = []
  arr.reverse_each { |i| reversed_arr << i }
  return reversed_arr
end

puts reverse_array([1, 2, 3, 4])  # Output: [4, 3, 2, 1]
```




