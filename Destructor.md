# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```
#Reg.NO-212222220027
#Name-MONIKA RV

class Student:
    def __init__(self):
        print("Constructor called: Student object created.")

    def __del__(self):
        print("Destructor called: Student object deleted.")

s2 = Student()
del s2



```

### OUTPUT
![image](https://github.com/user-attachments/assets/08734f1a-a2bb-4941-a427-2a84477d62ed)


### RESULT
Thus, the Python program using the Student class was successfully executed with a constructor and destructor, confirming that object creation and deletion work as expected.
