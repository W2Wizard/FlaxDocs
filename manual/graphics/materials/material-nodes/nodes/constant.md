# Constants

## Explanation

Constants, as the name implies, are values that cannot change once set in the material or when playing, unlike [properties](..\..\material-properties\index.md) and therefor won't be visible when creating a material instance.

Constants can be added, multiplied and merged to almost any other constant, for instance a float can be added with a vector3, as a result the single float value would be applied to X,Y and Z.

You can also multiply a boolean with a vector3 or add an integer to a color for example.

### **Float constant**

Floats in short simply describe a floating point number.

However, think of a float constant as a grayscale image, the closer to 0 the more darker the image would get and vice versa, the best way to visualize this is using a color gradient, here we can see 0 to 1 and all values in between. 

This is the basis for things like heightmaps, that describe each pixel as a value between 0 and 1.

![example](..\media\examples\constant-gradient-example.png)

### **Signed & Unsigned Integer constant**

Integers are denary numbers, the difference between signed and unsigned are that unsigned integers cannot go below 0. This comes from the fact that unsigned integers use a sign bit to signify if the number is negative or not, unsigned integers don't use that bit.

### **Bool constant**

A Bool constant, is just a simple true (1) or false (0) value.

### **PI constant**

PI is a vital number in mathematics and commonly used in calculations involved finding the area of a circle or its circumference and many other formulas.

### **Vector(2,3,4) constant**

The constant vector outputs the contains specified amount of channels as a float value, think of it like having multiple floats in 1 single type. They can be used to describe both a position or a color where each channel can represent R,G,B or A.

|    Vector      |           Description             |
| :------------: | :-------------------------------: |
|    Vector2     | Contains 2 channels: X & Y        |
|    Vector3     | Contains 3 channels: X, Y & Z     |
|    Vector4     | Contains 4 channels: X, Y, Z & W  |


### **Color constant**

A color constant is similar to a vector4 with the main difference being that its mainly purposed for colors as well as being able to use the color picker to determine the value.

## Example

In this example we can multiply a constant float with Texcoords, this results in a tiling effect, the higher the number

![example](..\media\examples\constant-example.png)

## Nodes

![nodes](..\media\nodes\constant-nodes.png)
