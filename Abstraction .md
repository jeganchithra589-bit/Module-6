# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod
import math

class type_shape(ABC):
    @abstractmethod
    def area(self):
        pass

# Rectangle class
class Rectangle(type_shape):
    def __init__(self, length, width):
        self.length = length
        self.width = width

    def area(self):
        return self.length * self.width

# Circle class
class Circle(type_shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return 3.14 * self.radius ** 2

# Square class
class Square(type_shape):
    def __init__(self, side):
        self.side = side

    def area(self):
        return self.side ** 2

# Triangle class
class Triangle(type_shape):
    def __init__(self, base, height):
        self.base = base
        self.height = height

    def area(self):
        return 0.5 * self.base * self.height

# Create objects
rect = Rectangle(6, 4)
circle = Circle(7)
square = Square(4)
triangle = Triangle(5, 4)

# Print results
print("Area of a rectangle:", rect.area())
print("Area of a circle:", circle.area())
print("Area of a square:", square.area())
print("Area of a triangle:", triangle.area())
```

## Output
<img width="1920" height="1080" alt="Screenshot (141)" src="https://github.com/user-attachments/assets/2d6a6be4-6daf-444a-bc52-07458aeac841" />

## Result
