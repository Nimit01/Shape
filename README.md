Shape Calculator

Overview

This Java program implements a menu-driven shape calculator that allows users to compute area, perimeter, and volume for different geometric shapes. The program follows object-oriented principles using abstract classes and interfaces.

Features

Calculate Area & Perimeter for:

Circle

Rectangle

Square

Sphere

Cylinder

Equilateral Pyramid (Square Base)

Calculate Volume for:

Sphere

Cylinder

Equilateral Pyramid

User-friendly menu-driven interface

Proper input validation

File Structure & Method Descriptions

**1. **Shape.java

Abstract class with common properties of all shapes.

Defines:

calculateArea(): Abstract method to calculate area.

calculatePerimeter(): Abstract method to calculate perimeter.

Shape(String shape): Non-abstract constructor to initialize shape properties.

**2. **Volume.java

Interface defining:

calculateVolume(): Abstract method for volume calculation.

**3. **Circle.java

Extends Shape, implements:

calculateArea(): Returns π * r².

calculatePerimeter(): Returns 2 * π * r.

**4. **Rectangle.java

Extends Shape, implements:

calculateArea(): Returns length * width.

calculatePerimeter(): Returns 2 * (length + width).

**5. **Square.java

Extends Shape, implements:

calculateArea(): Returns side².

calculatePerimeter(): Returns 4 * side.

**6. **Sphere.java

Extends Shape, Implements Volume, defines:

calculateArea(): Returns 4 * π * r².

calculatePerimeter(): Returns 2 * π * r (great circle circumference).

calculateVolume(): Returns (4/3) * π * r³.

**7. **Cylinder.java

Extends Shape, Implements Volume, defines:

calculateArea(): Returns 2 * π * r * (r + h).

calculatePerimeter(): Returns 2 * π * r (base circumference).

calculateVolume(): Returns π * r² * h.

**8. **EquilateralPyramid.java

Extends Shape, Implements Volume, defines:

calculateArea(): Returns base² + 2 * (base * slantHeight).

calculatePerimeter(): Returns 4 * base.

calculateVolume(): Returns (1/3) * base² * height.

**9. **Main.java

Implements menu-driven interface.

Asks users for shape selection and required dimensions.

Calls respective calculateArea(), calculatePerimeter(), and calculateVolume() methods.

How to Run

Clone the repository

git clone https://github.com/your-username/Shape_Calculator.git
cd Shape_Calculator

Compile the Java files

javac Main.java Shape.java Volume.java Circle.java Rectangle.java Square.java Sphere.java Cylinder.java EquilateralPyramid.java

Run the program

java Main

Exception Handling & Input Validation

This program ensures:

Valid numeric inputs are entered by users.

Invalid choices are handled gracefully in the menu.

No invalid calculations occur for shapes with missing dimensions.

Sample Output

Select Shape:
1. Circle
2. Rectangle
3. Square
4. Sphere
5. Cylinder
6. Equilateral Pyramid
7. Exit
Enter choice: 

Author

Name: [Nimit Prakash]

