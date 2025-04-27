# Exp.No:21  
## Constructors - Parameterized Constructor

### AIM  
To Write a python program using class to perform addition of three numbers using default constructor.Assume the three numbers are 
num1=1000
num2=2000
num3=3000

### ALGORITHM

1. Begin the program.
2. Define a class add with an __init__ method to initialize the variables num1, num2, and num3 with values 1000, 2000, and 3000 respectively.
3. Define a method dis() inside the class that: Calculates the sum of num1, num2, and num3, and assigns it to self.num.
4. Prints the value of self.num.
5. Create an object obj of the class add.
6. Call the dis() method on the obj object to display the sum.
7. Terminate the program.

### PROGRAM
```
class add:
    def __init__(self):
        self.num1=1000
        self.num2=2000
        self.num3=3000
    def dis(self):
        self.num=self.num1+self.num2+self.num3
        print(self.num)
obj=add()
obj.dis()
```
### OUTPUT
![Screenshot 2025-04-27 164940](https://github.com/user-attachments/assets/06ee6d93-5c4e-4f4f-b631-b0ee504ea586)

### RESULT
Thus a python program using class to perform addition of three numbers using default constructor has been successfully implemented.
