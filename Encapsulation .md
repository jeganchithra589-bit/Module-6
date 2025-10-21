# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    __length=15
    __breadth=2
    def sum(self,__length,__breadth):
        print("Area of Rectangle",__length*__breadth)

obj=Rectangle()
obj.sum(15,2)
```
## Output
<img width="1920" height="1080" alt="Screenshot (142)" src="https://github.com/user-attachments/assets/c05c8802-b458-4d8b-a3f2-233235aa7934" />

## Result
