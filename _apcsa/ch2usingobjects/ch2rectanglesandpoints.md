---
layout: project
category: ch2usingobjects
title: Ch2 Rectangles and Points
---

Skim Sections 2.1-2.2 (pages 31-40)
Check out the Rectangle class in the Java API:
  - [Java Rectangle class API](https://docs.oracle.com/javase/7/docs/api/index.html?java/awt/Rectangle.html)

Practice Exercises Page 72: 2.1, 2.5, 2.14

You will create ONE class with one public static void main() that contains code for the following 3 exercises.

## E2.1

Write an AreaTester program that constructs a Rectangle object.
Ask the user for a width and height.
Use the setSize method to adjust the width and height of your Rectangle object.
Finally, compute and print its area using the getWidth and getHeight methods.

## E2.5

Look into the API documentation of the Rectangle class and locate the method
<pre>
void add(int newx, int newy)
</pre>
Read through the method documentation. Then estimate the result of the following statements:
<pre>
Rectangle box = new Rectangle(5, 10, 20, 30);
</pre>
<pre>
box.add(0, 0);
</pre>
Print your *predicted* new X location, new Y location, new width, and new height. *NOTE: Your prediction CAN be inaccurate.*

Write a program that will...

  1.  Print your predicted X location for the final box
  1.  Print your predicted Y location for the final box
  1.  Print your predicted width for the final box
  1.  Print your predicted height for the final box
  1.  Instantiate a rectangle at 5, 10 that is 20 wide and 30 tall
  1.  Add the point 0, 0 to the rectangle
  1.  Print the actual X location (using the getX method) of the final box
  1.  Print the actual Y location (using the getY method) of the final box
  1.  Print the actual width (using getWidth method) of the final box
  1.  Print the actual height (using getHeight method) of the final box

## E2.14

[Java Point class API](https://docs.oracle.com/javase/7/docs/api/java/awt/Point.html)

Look at the API of the Point class and find out how to construct a Point object. In a PointTester program, construct two points with coordinates (3, 4) and (–3, –4). Find the distance between them, using the distance method (which is available because it is *inherited* from a different class). Print your prediction and then the calculated distance.
