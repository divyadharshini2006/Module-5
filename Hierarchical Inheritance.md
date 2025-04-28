# Exp.No:25  
## Hierarchical Inheritance

### AIM  
To Write a Python program to Get the Doctor  and patient details & display it using Hierarchical inheritance.
Note: create a parent (base) class name Details and two child (derived) classes named Doctor and Patient.

### ALGORITHM

1. Define the Details class.
2. Create the __init__ method to initialize id, name, and gender.
3. Create the setData method to set values of id, name, and gender.
4. Create the showData method to display id, name, and gender.
5. Define the Employee class inheriting from Details.
6. Create the __init__ method to initialize company and dept.
7. Create the setEmployee method to set employee details and inherited data.
8. Create the showEmployee method to display employee details and inherited data.
9. Define the Patient class inheriting from Details.
10. Create the __init__ method to initialize hospital and dept.
11. Create the setEmployee method to set patient details and inherited data.
12. Create the showEmployee method to display patient details and inherited data.
13. Take input for doctor details.
14. Take input for patient details.
15. Create an object of Employee class and set employee data.
16. Display employee details using showEmployee.
17. Create an object of Patient class and set patient data.
18. Display patient details using showEmployee.
19. Terminate the program.

### PROGRAM
```
# hierarchical inheritance

class Details:
    def __init__(self):
        self.__id="<No Id>"
        self.__name="<No Name>"
        self.__gender="<No Gender>"
    def setData(self,id,name,gender):
        self.__id=id
        self.__name=name
        self.__gender=gender
    def showData(self):
        print("Id: ",self.__id)
        print("Name: ", self.__name)
        print("Gender: ", self.__gender)

class Employee(Details): #Inheritance
    def __init__(self):
        self.__company="<No Company>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,comp,dept):
        self.setData(id,name,gender)
        self.__company=comp
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__company)
        print("Department: ", self.__dept)

class Patient(Details): #Inheritance
    def __init__(self):
        self.__hospital="<No Hospital>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,hos,dept):
        self.setData(id,name,gender)
        self.__hospital=hos
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__hospital)
        print("Department: ", self.__dept)

id=int(input())
name=input()
gender=input()
comp=input()
dept=input()
id1=int(input())
nam=input()
gen=input()
hosp=input()
dep=input()

print("Doctor Object")
e=Employee()
e.setEmployee(id,name,gender,comp,dept)
e.showEmployee()
print("\nPatient Object")
d = Patient()
d.setEmployee(id1, nam, gen, hosp, dep)
d.showEmployee()

```
### OUTPUT  
![Screenshot 2025-04-28 151155](https://github.com/user-attachments/assets/473058f9-df33-4c4a-9ef9-1e047e2bc3fa)

### RESULT
Thus a Python program to Get the Doctor  and patient details & display it using Hierarchical inheritance has been implemented successfully.

