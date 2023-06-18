## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?
Ans: Python is called a general purpose language because it can be used for a wide variety of tasks, including:Web development,Data science,System administration,Scientific computing.Python is also called a high-level language because it is closer to human language than low-level languages, such as assembly language. This makes Python easier to read and write, and it also makes it more portable, meaning that Python code can be run on different platforms without modification.
Python is considered a high-level programming language because of its features too like Abstraction,Simplicity,Community Support, Simplicity.

Q2. Why is Python called a dynamically typed language?
Ans: Python is a dynamically typed language because the data type of a variable is not declared before it is used. This means that the type of the variable can be changed at any time, and the compiler will automatically adjust its behavior accordingly. Dynamic typing can make Python code more concise and easier to read, but it can also lead to errors if the programmer is not careful.

Q3. List some pros and cons of Python programming language?
Ans: Pros: 1. Easy to learn and use: Python has a simple syntax that is easy to learn and understand, making it a good choice for beginners.
2. Powerful and versatile: Python is a powerful language that can be used for a wide variety of tasks, including web development, data science, and machine learning.
3. Large and active community: Python has a large and active community of developers who provide support and resources.
Cons:
1. Not as fast as some other languages: Python is not as fast as some other languages, such as C or C++.
2. Not as memory efficient as some other languages: Python is not as memory efficient as some other languages, such as C or C++.
3. Can be difficult to debug: Python can be difficult to debug, especially for beginners.

Q4. In what all domains can we use Python?
Ans: Web Development, Data Science, Scientific Computing, Machine learning, System Administration,Artificial Intelligence, Game Development etc.

Q5. What are variable and how can we declare them?
Ans: A variable is a storage location that can be assigned a value. Variables are used to store data so that it can be used later. In Python, variables are declared using the following syntax: variable_name = value

Q6. How can we take an input from the user in Python?
Ans: The input() function takes a prompt as its argument and returns the user's input as a string. 

Q7. What is the default datatype of the value that has been taken as an input using input() function?
Ans: The default data type of the value that has been taken as an input using input() function in Python language is string.The input() function in Python takes a string as an input and returns a string. This means that if you enter a number, it will be converted to a string before it is returned.

Q8. What is type casting?
Ans : Type casting also called as data type conversion, is the process of converting a value from one data type to another.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
Ans: No, we cannot take more than one input from the user using a single input() function. The input() function in Python takes a string as an input and returns a string. This means that if you enter multiple values, they will be interpreted as a single string. 

Q10. What are keywords?
Ans: keywords are reserved words that have a special meaning to the Python interpreter. They are used to control the flow of execution and to define the structure of a program. Keywords cannot be used as variable names, function names, or any other identifier.

Q11. Can we use keywords as a variable? Support your answer with reason.
Ans: No we cannot use keywords as a variable in Python language. Keywords are reserved words that have a special meaning to the Python interpreter.

Q12. What is indentation? What's the use of indentaion in Python?
Ans: Indentation in Python refers to the spaces at the beginning of a code line. Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important. Python uses indentation to indicate a block of code. 

Q13. How can we throw some output in Python?
Ans: We use the print() function. The print() function takes any number of arguments and prints them to the console.

Q14. What are operators in Python?
Ans: Operators in Python are special symbols that perform operations on values. They can be used to perform arithmetic operations, logical operations, and membership operations.Some of the key operators in Arithmetic operators,Assignment operators,Comparison operators,Logical operators,Identity operators,Membership operators,Bitwise operators.

Q15. What is difference between / and // operators?
Ans: The difference between the / and // operators in Python is that the / operator performs floating-point division, while the // operator performs integer division.

Q16. Write a code that gives following as an output.
     "iNeuroniNeuroniNeuroniNeuron"
Ans: for i in range(5):
         print("iNeuron", end="")

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
Ans: 
      number = int(input("Enter a number: "))
if number % 2 == 0:
    print("The number is even")
else:
    print("The number is odd")


Q18. What are boolean operator?
Ans: Boolean operators are operators that are used to combine Boolean values. Boolean values can be either True or False. The three most common Boolean operators are:
      1. AND: The AND operator returns True if both of its operands are True.
      2. OR: The OR operator returns True if either of its operands is True.
      3. NOT: The NOT operator returns the opposite of its operand.

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0

Ans: 1 or 0 -> 1 ; 0 and 0 -> 0 ; True and False and True -> False; 1 or 0 or 0 -> 1

Q20. What are conditional statements in Python?
Ans: Conditional statements are used to control the flow of execution in a Python program. They allow you to execute different code depending on whether a certain condition is true or false.There are three types of conditional statements in Python:
1. If statement: The if statement is the most basic conditional statement. It allows you to execute a block of code if a certain condition is true.
2. Elif statement: The elif statement is used to chain multiple if statements together. It allows you to execute a block of code if a certain condition is true, but only if the previous if statement was not true.
3. Else statement: The else statement is used to execute a block of code if none of the previous if or elif statements were true.

Q21. What is use of 'if', 'elif' and 'else' keywords?
Answer: The if, elif, and else keywords are used to create conditional statements in Python. Conditional statements allow you to execute different code depending on whether a certain condition is true or false.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
Ans: age = int(input("Enter your age: "))
            if age >= 18:
               print("You can vote.")
            else:
               print("You can't vote.")


Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans:
numbers = [12, 75, 150, 180, 145, 525, 50]
even_sum = 0
for number in numbers:

    if number % 2 == 0:
        even_sum += number
print("The sum of even numbers is:", even_sum)


Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
Ans: 
num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))
num3 = int(input("Enter the third number: "))

greatest_number = max(num1, num2, num3)
print("The greatest number is:", greatest_number)


Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans: numbers = [12, 75, 150, 180, 145, 525, 50]

for number in numbers:
    # Check if the number is divisible by five
    if number % 5 == 0:
        # Check if the number is greater than 150
        if number > 150:
            # Skip the number
            continue
        # Check if the number is greater than 500
        if number > 500:
            # Stop the loop
            break
        # Print the number
        print(number)
