📐 **Area, Perimeter and Volume Finder**

A Python-based geometry calculator that calculates area, perimeter, surface area, and volume for different 2D and 3D shapes.

✨ **Features**

- Supports 11 different shapes
- Calculates area and perimeter for 2D shapes
- Calculates surface area and volume for 3D shapes
- Supports repeated calculations using a "while" loop
- Type "exit" to close the program
- Accepts decimal values using "float()"
- Handles both lowercase and capitalized shape names

📚 **Supported Shapes**

**2D Shapes**

- Square
- Rectangle
- Circle
- Triangle
- Semicircle

**3D Shapes**

- Cube
- Cuboid
- Sphere
- Cylinder
- Hemisphere
- Cone

🧮 **Calculations**

The program uses standard mathematical formulas for each shape.

**For example:**

- Square → Area and Perimeter
- Circle → Area and Circumference
- Triangle → Area and Perimeter
- Cube → Surface Area and Volume
- Cuboid → Surface Area and Volume
- Cone → Curved Surface Area, Total Surface Area and Volume

▶️ **How to Run**

1. Make sure Python 3 is installed.
2. Run the Python file.
3. Enter the name of a shape.
4. Enter the required dimensions.
5. View the calculated result.
6. Type "exit" when you want to close the program.

**Example**

Enter the shape circle
Enter the Radius 7
The area is: 154.0
The perimeter or circumference is: 44.0 

🛠️ **Concepts Used**

This project was made using basic Python concepts:

- "print()"
- "input()"
- Variables
- "float()"
- Arithmetic operators
- "if / elif / else"
- "while True"
- "break"

🎯 **Purpose**

This project was created as a Python practice project to improve conditional logic, loops, mathematical calculations, and problem-solving skills.

👨‍💻 **Author**

**Garv (GitHub: Garv725)** 

**Built with 🐍 Python 3**

```python
print("="*60)
print("Area,Perimeter and Volume Finder")
print("="*60)

while True:
    shape = str(input("Enter the shape "))
    if shape == 'exit':
        break
    elif shape == 'square' or shape == 'Square':
        length = input("Enter the Length of the side ")
        if length == 'exit':
            break
        else:
         length = float(length)
         print("The area is:",length*length)
         print("The perimeter is:",4*length)
    elif shape == 'rectangle' or shape == 'Rectangle':
        length = input("Enter the Length ")
        if length == 'exit':
            break
        else:
          length = float(length)
          breadth = input("Enter the Breadth ")
        if breadth == 'exit':
            break
        else:
            breadth = float(breadth)
            print("The area is:",length*breadth)
            print("The perimeter is:",2*(length+breadth))
    elif shape == 'cube' or shape == 'Cube':
        length = input("Enter the Length of the side ")
        if length == 'exit':
            break
        else:
          length = float(length)
          print("The area is:",6*(length**2))
          print ("The volume is:",length**3)
    elif shape == 'cuboid' or shape == 'Cuboid':
        length = input("Enter the Length ")
        if length == 'exit':
            break
        else:
          length = float(length)
          breadth = input("Enter the Breadth ")
        if breadth == 'exit':
            break
        else:
            breadth = float(breadth)
            height = input("Enter the Height ")
        if height == 'exit':
            break
        else:
            height = float(height)
            print("The area is:",2*(length*breadth + breadth*height + height*length))
            print ("The volume is:",length*breadth*height)
    elif shape == 'circle' or shape == 'Circle':
        length = input("Enter the Radius ")
        if length == 'exit':
                break
        else:
              length = float(length)
              print("The area is:",22/7*(length**2))
              print("The perimeter or circumference is:",2*22/7*length) 
    elif shape == 'triangle' or shape == 'Triangle':
        length = input("Enter the Length of first side ")
        if length == 'exit':
            break
        else:
              length = float(length)
              breadth = input("Enter the Length of second side ")
        if breadth == 'exit':
            break
        else:
            breadth = float(breadth)
            height = input("Enter the Length of third side ")
        if height == 'exit':
            break
        else:
            height = float(height)
            per_height = input("Enter the Perpendicular Height ")
        if per_height == 'exit':
            break
        else:
            per_height = float(per_height)
            print ("The area is:",1/2*length*per_height)
            print ("The perimeter is:",length+breadth+height)
    elif shape == 'sphere' or shape == 'Sphere':
        length = input("Enter the Radius ") 
        if length == 'exit':
            break
        else:
              length = float(length)
              print("The area is:",4*22/7*(length**2))
              print ("The volume is:",4/3*22/7*(length**3))
    elif shape == 'semicircle' or shape == 'Semicircle':
        length = input("Enter the Radius ")
        if length == 'exit':
            break
        else:
              length = float(length)
              print("The area is:",1/2*22/7*(length**2))
              print ("The perimeter or circumference is:",length*(22/7+2))
    elif shape == 'cylinder' or shape == 'Cylinder':
        length = input("Enter the Radius ")
        if length == 'exit':
            break
        else:
              length = float(length)
              height = input("Enter the Height ")
        if height == 'exit':
            break
        else:
            height = float(height)
            print ("The area is:",2*22/7*length*(length+height))
            print ("The volume is:",22/7*(length**2)*height)
    elif shape == 'hemisphere' or shape == 'Hemisphere':
        length = input("Enter the Radius ")
        if length == 'exit':
            break
        else:
              length = float(length)
              print ("The curved surface area is:",2*22/7*(length**2))
              print ("The total surface area is:",3*22/7*(length**2))
              print ("The volume is:",2/3*22/7*(length**3))
    elif shape == 'cone' or shape == 'Cone':
        length = input("Enter the Radius ")
        if length == 'exit':
            break
        else:
              length = float(length)
              breadth = input("Enter the Slant Height ")
        if breadth == 'exit':
            break
        else:
            breadth = float(breadth)
            height = input("Enter the Perpendicular Height ")
        if height == 'exit':
            break
        else:
            height = float(height)
            print("The curved surface area is:",22/7*length*breadth)
            print ("The total surface area is:",22/7*length*(breadth + length))
            print ("The volume is:",1/3*22/7*(length**2)*height)
    else:
        print("Invalid! ")

