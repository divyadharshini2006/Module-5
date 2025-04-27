# Exp.No:25  
## Hierarchical Inheritance

### AIM  
To Write A Python Program to Calculated Add, Sub, & Mul using Inheritance.

### ALGORITHM

1. Begin the program.
2. Define a class Addition with:
3. An __init__() method to initialize two values a and b.
4. A method add() that prints the values a, b, and their sum.
5. Define a class Multiplication that inherits from Addition with:
6. A method multiply() that prints the values a, b, and their product.
7. Define a class Subtraction that inherits from Multiplication with:
8. A method subtract() that prints the values a, b, and their difference.
9. Take two integer inputs a and b from the user.
10. Create an object obj of the Subtraction class (which has access to all methods).
11. Call the add(), multiply(), and subtract() methods on the obj object to display the respective results.
12.Terminate the program.

### PROGRAM
```
class Addition:
    def __init__(self, a, b):
        self.a = a
        self.b = b
    
    def add(self):
        print(" Addition value1 : ", self.a)
        print(" Addition value2 : ", self.b)
        print(" Added value :", self.a + self.b)

class Multiplication(Addition):
    def multiply(self):
        print(" multiplication value1 : ", self.a)
        print(" multiplication value2 : ", self.b)
        print(" Multiplied value :", self.a * self.b)

class Subtraction(Multiplication):
    def subtract(self):
        print(" subraction value1 : ", self.a)
        print(" subraction value2 : ", self.b)
        print("Subracted value :", self.a - self.b)

# Taking input from the user
a = int(input())
b = int(input())

# Creating an object of Subtraction class (which has access to all methods)
obj = Subtraction(a, b)
obj.add()
obj.multiply()
obj.subtract()
```

### OUTPUT  
![Screenshot 2025-04-27 165747](https://github.com/user-attachments/assets/5eca765f-8b7a-4288-a791-d36f31eca2b0)

### RESULT
Thus a Python Program to Calculated Add, Sub, & Mul using Inheritance has been successfully implemented .

