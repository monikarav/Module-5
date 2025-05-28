# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```


class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def display_details(self):
        print(f"ID: {self.id}")
        print(f"Name: {self.name}")
        print(f"Gender: {self.gender}")

class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def display_details(self):
        print("\n--- Employee Details ---")
        super().display_details()
        print(f"Company: {self.company}")
        print(f"Department: {self.department}")

class Doctor(Details):
    def __init__(self, id, name, gender, hospital, department):
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def display_details(self):
        print("\n--- Doctor Details ---")
        super().display_details()
        print(f"Hospital: {self.hospital}")
        print(f"Department: {self.department}")

# Taking input for Employee
print("Enter Employee Details:")
eid = input("ID: ")
ename = input("Name: ")
egender = input("Gender: ")
ecompany = input("Company: ")
edepartment = input("Department: ")
emp = Employee(eid, ename, egender, ecompany, edepartment)

# Taking input for Doctor
print("\nEnter Doctor Details:")
did = input("ID: ")
dname = input("Name: ")
dgender = input("Gender: ")
dhospital = input("Hospital: ")
ddepartment = input("Department: ")
doc = Doctor(did, dname, dgender, dhospital, ddepartment)

# Displaying the details
emp.display_details()
doc.display_details()


```

### OUTPUT  

![image](https://github.com/user-attachments/assets/2e4170d4-3c73-4b2e-b8e7-ad3e5272ad7c)



### RESULT
Thus, the python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named Details and two child (derived) classes named Employee and Doctor has been executed and verified successfully.
