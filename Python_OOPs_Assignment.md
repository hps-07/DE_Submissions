Q1. What is the purpose of Python's OOP?
The purpose of Python's OOP is to provide a way to organize code into reusable objects. This makes code more modular, easier to understand, and easier to maintain.

Q2. Where does an inheritance search look for an attribute?
An inheritance search looks for an attribute in the following order:
1. The current object's instance attributes
2. The current object's class attributes
3. The parent class's instance attributes
4. The parent class's class attributes
5. And so on, up the inheritance chain

Q3. How do you distinguish between a class object and an instance object?
A class object is a blueprint for creating instances. It contains the code for the instance's methods and attributes. An instance object is a specific object that was created from a class. It inherits the methods and attributes from its class.

Q4. What makes the first argument in a class’s method function special?
The first argument in a class's method function is always the instance object itself. It is usually named `self`.

Q5. What is the purpose of the init method?
The init method is a special method that is called when an instance of a class is created. It is used to initialize the instance's attributes.

Q6. What is the process for creating a class instance?
To create a class instance, you use the `__init__()` method. The `__init__()` method is a special method that is called when an instance of a class is created. It is used to initialize the instance's attributes.

Q7. What is the process for creating a class?
To create a class, you use the `class` keyword. The `class` keyword is used to define a new class. The syntax for creating a class is as follows:

class ClassName:
    # class body

The `class body` is a block of code that contains the code for the class's methods and attributes.

Q8. How would you define the superclasses of a class?
The superclasses of a class are the classes that the class inherits from. The superclasses of a class are defined in the class's `__init__()` method.

Q9. What is the relationship between classes and modules?
Classes and modules are both ways of organizing code. Modules are used to organize code that is not related to each other. Classes are used to organize code that is related to each other.

Q10. How do you make instances and classes?
To make instances and classes, you use the `__init__()` method and the `class` keyword. The `__init__()` method is used to create instances. The `class` keyword is used to create classes.

Q11. Where and how should be class attributes created?
Class attributes should be created in the class's `__init__()` method. Class attributes are defined outside of any methods.

Q12. Where and how are instance attributes created?
Instance attributes should be created in the `__init__()` method. Instance attributes are defined inside of methods.

Q13. What does the term "self" in a Python class mean?
The term "self" in a Python class refers to the current instance of the class.

Q14. How does a Python class handle operator overloading?
A Python class can handle operator overloading by defining special methods for the operators that it wants to overload. For example, the `__add__()` method can be used to overload the addition operator.

Q15. When do you consider allowing operator overloading of your classes?
You should consider allowing operator overloading of your classes when you want to provide a more intuitive way for users of your class to interact with it. For example, you might want to allow users of your class to add two instances of your class together.

Q16. What is the most popular form of operator overloading?
The most popular form of operator overloading is the use of special methods to overload the arithmetic operators.

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?
The two most important concepts to grasp in order to comprehend Python OOP code are inheritance and polymorphism. Inheritance is the ability of a class to inherit the attributes and methods of another class. Polymorphism is the ability of objects of different types to respond to the same message in the same way.

Q18. Describe three applications for exception processing.
There are many applications for exception processing in Python. Here are three examples:
1. To handle errors that occur during runtime.For example, if a user tries to divide by zero, an exception will be raised. The exception can be handled by using a try-except block.
2. To control the flow of execution. For example, you can use exceptions to exit a loop or to skip a certain section of code.
3. To create custom errors: You can create custom errors to represent specific types of errors that occur in your code. This can make your code more readable and easier to debug.

Q19. What happens if you don't do something extra to treat an exception?
If you don't do something extra to treat an exception, the default behavior is to print a stack trace and exit the program. This can be very frustrating for users, so it's important to handle exceptions gracefully.

Q20. What are your options for recovering from an exception in your script?
There are many ways to recover from an exception in your script. Here are a few options:
1. Print a message to the user: This can be helpful for debugging or for letting the user know what happened.
2. Log the exception to a file: This can be helpful for tracking down errors in your code.
3. Re-raise the exception: This can be useful if you want to handle the exception in a different part of your code.
4. Ignore the exception : This should only be done as a last resort, as it can lead to unexpected behavior in your code.

Q21. Describe two methods for triggering exceptions in your script.
There are two main methods for triggering exceptions in your script:
1. Using the `raise` statement: The `raise` statement can be used to raise an exception explicitly.
2. Using the `assert` statement: The `assert` statement can be used to check a condition. If the condition is false, an exception will be raised.

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of whether or not an exception exists.
There are two main methods for specifying actions to be executed at termination time, regardless of whether or not an exception exists:
1. Using the `finally` clause : The `finally` clause is a block of code that is executed regardless of whether or not an exception is raised.
2. Using the `atexit` module: The `atexit` module provides a way to register functions that will be executed when the program exits.

Q23. What is the purpose of the try statement?
The try statement is used to execute a block of code and handle any exceptions that may occur. The syntax for a try statement is as follows:

try:
    # block of code to be executed
except Exception as e:
    # handle the exception

The `try` block is executed first. If an exception occurs in the `try` block, the `except` block is executed. The `Exception` object can be used to get more information about the exception.

Q24. What are the two most popular try statement variations?
The two most popular try statement variations are the `except` clause and the `finally` clause.The `except` clause is used to handle exceptions that occur in the `try` block. The `finally` clause is executed regardless of whether or not an exception occurs.

Q25. What is the purpose of the raise statement?
The raise statement is used to raise an exception explicitly. The syntax for the raise statement is as follows:

raise Exception("message")

The `Exception` object can be used to specify the type of exception that is raised. The `message` argument can be used to provide more information about the exception.

Q26. What does the assert statement do, and what other statement is it like?
The assert statement is used to check a condition. If the condition is false, an AssertionError exception is raised. The assert statement is similar to the if statement, but it is used to check for errors in your code.

Q27. What is the purpose of the with/as argument, and what other statement is it like?
The with/as statement is used to ensure that resources are properly closed when they are no longer needed. The with/as statement is similar to the try/finally statement, but it is specifically designed for managing resources.

Q28. What are *args, **kwargs?
*args and **kwargs are special parameters that can be used to pass a variable number of arguments to a function. *args is used to pass a variable number of positional arguments, and **kwargs is used to pass a variable number of keyword arguments.

Q29. How can I pass optional or keyword parameters from one function to another?
Optional or keyword parameters can be passed from one function to another by using the *args and **kwargs parameters. The *args parameter can be used to pass a variable number of positional arguments, and **kwargs can be used to pass a variable number of keyword arguments.

Q30. What are Lambda Functions?
Lambda functions are small, anonymous functions that can be used to perform simple tasks. Lambda functions are created using the lambda keyword.

Q31. Explain Inheritance in Python with an example?
Inheritance is the ability of a class to inherit the attributes and methods of another class. This allows you to reuse code and make your code more modular.
Here is an example of inheritance in Python:

class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        print("I am an animal!")

class Dog(Animal):
    def bark(self):
        print("Woof!")

my_dog = Dog("Fido")
my_dog.speak()  # Prints "I am an animal!"
my_dog.bark()  # Prints "Woof!"

In this example, the Dog class inherits from the Animal class. This means that the Dog class has all of the attributes and methods of the Animal class, plus its own additional attributes and methods.

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of class C, which version gets invoked?
If we call func() from an object of class C, the version of func() that is defined in class C will be invoked. This is because class C inherits from classes A and B, so the version of func() that is defined in class C is the most specific version.

Q33. Which methods/functions do we use to determine the type of instance and inheritance?
The type() function can be used to determine the type of an instance. The isinstance() function can be used to check if an instance is of a specific type. The issubclass() function can be used to check if a class is a subclass of another class.

Q34.Explain the use of the 'nonlocal' keyword in Python.
The nonlocal keyword is used to declare a variable that is not local to the current scope. This means that the variable can be accessed from nested scopes.

Q35. What is the global keyword?
The global keyword is used to declare a variable that is global to the current module. This means that the variable can be accessed from anywhere in the module.


