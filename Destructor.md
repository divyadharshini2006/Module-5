# Exp.No:22  
## Destructor

### AIM  
To Add the destructor in the following python code to delete the instance of the class.

### ALGORITHM

1. Begin the program.
2. Define a class Student with:
3. An __init__() method that initializes name and age attributes.
4. A printDetail() method that prints the student's name and age.
5. A __del__() method that prints a message indicating the student object is deleted.
6. Create an object s1 of the Student class, passing "Vishvajit Rao" as the name and 22 as the age.
7. Call the printDetail() method on s1 to print the student's details.
8. Delete the s1 object using del s1, triggering the __del__() method.
9. Terminate the program.

### PROGRAM
```
class Student:
	def __init__(self, name, age):
		self.name = name
		self.age = age

	def printDetail(self):
		print(f"My name is {self.name} and I am {self.age} years old.")

	def __del__(self):
	    print(f"{self.name} student is deleted.")


s1 = Student("Vishvajit Rao", 22)
s1.printDetail()
del s1
```
### OUTPUT
![Screenshot 2025-04-27 165149](https://github.com/user-attachments/assets/99af972d-6c00-4279-8169-5ed0f1083f4e)
### RESULT
Thus Add the destructor in the following python code to delete the instance of the class has been successfully implemented.
