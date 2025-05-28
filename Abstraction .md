#  Python OOP: Abstract Class & Method Example

##  AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

##  ALGORITHM

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

##  Program
```python

from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def calculate_area(self): pass

class Rectangle(Shape):
    def calculate_area(self): return 5 * 3  # 15

class Circle(Shape):
    def calculate_area(self): return 3.14 * 4**2  # 50.24

print("Area of a rectangle:", Rectangle().calculate_area())
print("Area of a circle:", Circle().calculate_area())

```
## Output
![image](https://github.com/user-attachments/assets/743a284a-88d9-462c-a7dc-2f18d3876382)

## Result
Thus, the program is executed successfully
