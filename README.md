# Shape Calculator

## 📌 Overview
This Java program implements a **menu-driven shape calculator** that allows users to compute **area, perimeter, and volume** for different geometric shapes. The program follows **object-oriented principles** using **abstract classes and interfaces**.

## ✨ Features
- **Calculate Area & Perimeter for:**
  - Circle
  - Rectangle
  - Square
  - Sphere
  - Cylinder
  - Equilateral Pyramid (Square Base)
- **Calculate Volume for:**
  - Sphere
  - Cylinder
  - Equilateral Pyramid
- **User-friendly menu-driven interface**
- **Proper input validation**

## 📂 File Structure & Method Descriptions

### **1. `Shape.java`** (Abstract Class)
- Defines:
  - `calculateArea()` ➜ **Abstract method to calculate area**
  - `calculatePerimeter()` ➜ **Abstract method to calculate perimeter**
  - `Shape(String shape)` ➜ **Non-abstract constructor to initialize shape properties**

### **2. `Volume.java`** (Interface)
- Defines:
  - `calculateVolume()` ➜ **Abstract method for volume calculation**

### **3. `Circle.java`**
- Implements:
  - `calculateArea()` ➜ **Returns `π * r²`**
  - `calculatePerimeter()` ➜ **Returns `2 * π * r`**

### **4. `Rectangle.java`**
- Implements:
  - `calculateArea()` ➜ **Returns `length * width`**
  - `calculatePerimeter()` ➜ **Returns `2 * (length + width)`**

### **5. `Square.java`**
- Implements:
  - `calculateArea()` ➜ **Returns `side²`**
  - `calculatePerimeter()` ➜ **Returns `4 * side`**

### **6. `Sphere.java`**
- Implements:
  - `calculateArea()` ➜ **Returns `4 * π * r²`**
  - `calculatePerimeter()` ➜ **Returns `2 * π * r`**
  - `calculateVolume()` ➜ **Returns `(4/3) * π * r³`**

### **7. `Cylinder.java`**
- Implements:
  - `calculateArea()` ➜ **Returns `2 * π * r * (r + h)`**
  - `calculatePerimeter()` ➜ **Returns `2 * π * r`**
  - `calculateVolume()` ➜ **Returns `π * r² * h`**

### **8. `EquilateralPyramid.java`**
- Implements:
  - `calculateArea()` ➜ **Returns `base² + 2 * (base * slantHeight)`**
  - `calculatePerimeter()` ➜ **Returns `4 * base`**
  - `calculateVolume()` ➜ **Returns `(1/3) * base² * height`**

### **9. `Main.java`**
- Implements **menu-driven interface**
- Asks users for shape selection and required dimensions
- Calls respective `calculateArea()`, `calculatePerimeter()`, and `calculateVolume()` methods

## 🚀 How to Run
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Shape_Calculator.git
   cd Shape_Calculator
