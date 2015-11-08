# Introduction

Processing is all about learning to use code to draw on screen. The language is certainly capable of so much more than that, but this tutorial is going to focus on graphics.

## Download and install Processing

The download and installation process might be a litte different than you're used to, but please keep in mind this the Raspberry Pi implementation of Processing is brand new and it may take time for the process to become more streamlined.

1. Open the termminal window and enter the following command at the prompt to download and install Processing onto your Raspberry Pi:

		curl http://sukzessiv.net/~gohai/p5-arm/install-arm.sh | sudo sh

1. When the installation is complete, enter the following the command to start the Processing development environment:

		processing

## Write your first Processing sketch

The main Processing window is where you'll type your code. The Run button is how you'll execute that code. In the world of Processing, the program you write is called a **sketch**. Create your first simple sketch:

1. Enter the following code in the window:

	```java
	line(0,0,100,100);
	```

1. Click on the Run button. A new window should appear with a box and a diagonal line.

	The [line function](https://processing.org/reference/line_.html) draws a line between two points in the window. It takes four inputs: `x1`, and `y1` for the start of the line and `x2`, and `y2` for the end of the line. Its syntax is:

	```java
	line(x1, y1, x2, y2);
	```

	To understand what this means, you'll need to know that Processing uses a coordinate system like the one shown below; crucially the numbering begins at 0, not 1. Also, the origin is in the top left rather than the bottom left as you may be used to.

1. Try entering different values into the line function and press play. Below are a few ideas to try. Can you guess what the output will look like _before_ you execute the code?

	```java
	line(0,50,100,50);
	line(50,0,50,100);
	line(90,10,10,90);
	```

1. Processing will execute one line of code at a time, starting at the top of the sketch and working downward. This is called **procedural programming**. Try calling the `line` function a few different times with a few different values in a single sketch.

1. When you click Run, you'll notice that Processing draws each line you entered on the window.

## Draw other shapes

Of course, you can do a lot with lines, but Processing can draw a lot of different shapes. In these steps, you'll learn how to draw a circle and a rectangle.

1. Enter the following code in a blank sketch and press run:

	```java
	ellipse(50,15,30,30);
	```

	The [ellipse function](https://processing.org/reference/ellipse_.html) draws an ellipse (oval). An ellipse with equal width and height is more commonly known as a circle. The syntax for the ellipse function is:

	```java
	ellipse(xPosition, yPosition, width, height);
	```
1. Try changing the values of the ellipse and running your sketch to see how each value affects the shape.

1. If you go back to the original ellipse you drew, it looked like the start of a stick figure, don't you think? Try using the line function to draw the rest of the person. Here's a hint to get you started:


	```java
	ellipse(50,15,30,30);
	line(50,30,50,70);
	```

1. Even though you can draw a rectangle using just four lines, there's a [rectangle function](https://processing.org/reference/rect_.html) to make it easer. Its syntax is:

	```java
	rect(xPosition, yPosition, width, height);
	```

1. Try drawing a box around your stick figure. At this stage, it's important to note that as your code is executed, Processing draws shapes on top of previously-drawn shapes. Therefore, you may want to execute the `rect` function before the code to draw your stick figure.


## Make things move

## What next?

Learn how to use Processing for physical computing.

Processing for Raspberry Pi has been enhanced to use the Pi's GPIO pins. If you're interested in adding some physical interactivity to your project, then move onto [the next tutorial here](worksheet-2.md)
