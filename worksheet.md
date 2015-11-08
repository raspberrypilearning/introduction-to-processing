# Introduction

Processing is all about learning to use code to draw on screen. The language is certainly capable of so much more than that, but this tutorial is going to focus on graphics.

## Downloading and installing Processing

The download and installation process might be a litte different than you're used to, but please keep in mind this the Raspberry Pi implementation of Processing is brand new and it may take time for the process to become easier.

1. Open the termminal window and enter the following command at the prompt to download and install Processing onto your Raspberry Pi:

		curl http://sukzessiv.net/~gohai/p5-arm/install-arm.sh | sudo sh

1. When the installation is complete, enter the following the command to start the Processing IDE:

		processing

## Your first Processing sketch

The main Processing window is where you'll type code. The Run button is how you'll execute that code. In the world of Processing, the program you write is called a **sketch**. Create your first simple sketch:

1. Enter the following code in the window:

	```java
	line(0,0,100,100);
	```

1. Click on the Run button. A new window should appear with a box and a diagonal line.

## What next?

Learn how to use Processing for physical computing.

Processing for Raspberry Pi has been enhanced to use the Pi's GPIO pins. If you're interested in adding some physical interactivity to your project, then move onto [the next tutorial here](worksheet-2.md)
