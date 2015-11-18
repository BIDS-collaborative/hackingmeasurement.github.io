---
title: "Hands-on: Get Sensor Data from your Arduino!"
author: Dav Clark
presenters: Javier Rosa, Dav Clark
layout: class
---
## Required Software

This stuff is critical for one team-member to have ready on their laptop, but
the more the merrier!

 - Download and install the [Arduino
   IDE](https://www.arduino.cc/en/Main/Software).
 - Ensure you have Python 2.7 installed with PySerial. The easiest way to do
   this (on Windows, Mac, or Linux) is with [Continuum
   Anaconda](http://continuum.io/downloads).
 - [Fritzing](http://fritzing.org/home/).

## Reading

 - Read a little about Arduino on [the official
   site](https://www.arduino.cc/en/Guide/HomePage).
 - If you're curious for more detail, we're working with *clones* of the [open
   hardware](https://en.wikipedia.org/wiki/Open-source_hardware) [Arduino
   UNOs](https://www.arduino.cc/en/Main/ArduinoBoardUno).
 - *Alternatively* here's [a nice one-page intro to
   Arduino](http://teachmetomake.com/wordpress/arduino-hands-on-intro-workshop)
   from [Teach me to Make](http://teachmetomake.com/).

## Announcements

NOTE NEW TIME for event at [ManyLabs](https://www.manylabs.org/):

 - Work party *next Wednesday*, September 10 at 6pm [at
   ManyLabs](https://www.google.com/maps/place/Manylabs/@37.777164,-122.407709,17z/data=!4m3!3m2!1s0x80858082235da2e7:0xb30be4b717ffde73!4b1).
   We will be building plant boxes for 2nd graders that will be rolled from the
   exhibit space to outside.

## Review of expectations / updated syllabus

I've added greater clarity around grading on [the syllabus
page](syllabus.html). We'll review this briefly at the beginning of class. In
particular, be sure that I have your GitHub ID [using this
issue](https://github.com/BIDS-collaborative/hackingmeasurement.github.io/issues/33),
and that you've joined the Gitter chat room (linked at the footer of every page
on the site).

## Hands-on with Arduinos

We've had a conceptual introdution, but this week, we'll start programming and
getting data. A limited number of kits will be available, and priority will be
given to individuals who are formally enrolled in the course and/or on project
teams.

You can get a kit of your own for cheap, and this is encouraged! This way you
can engage more easily in your own projects and feel more free to do anything
you dream up. Let us know if you want help ordering (you can find us on the
Gitter chat, linked in the footer below).

## Tentative plan

We'll see how far we get, and move what's left to a later class:

 - Interfacing the Arduino™ with basic sensors (using Arduino C)
 - Getting data from an Arduino to a computer with SD cards
 - Bridging to Arduinos with serial

> Instructions: Navigate to https://github.com/BIDS-collaborative/hackingmeasurement.github.io/blob/gh-pages/syllabus/_posts/2015-09-10-hands-on-arduino.md and edit with the pencil icon/button.

> Also - before this will work for you, you need to accept the invitation to the github repo. Look here: https://github.com/BIDS-collaborative (there will be a link to the invitation near the top of the page)

# Hacking Measurement

Third meeting: 9/10/2015

# Agenda
 * Grading
 * Syllabus
 * More action on Tuesdays! (At BIDS Lab)
 * Learn more about Arduino

## Annoucements
 * Office hours on Tuesday (3:30 PM - 6:00 PM) - Just mention that you are here for the BIDS collaborative
 * Tuesday is time for team work!

### Arduino : An Introduction
 * Helps to know some basic C programming
 * Sensors for today:
        - Fingers!
        - Motion (PIR) sensor
        - Accelerometer
        - Water temperature sensor
 * Ardunio is open source, a lot of helpful libraries are available online.
 * Go to Tools -> Board and choose "Arduino Uno" for the type of Arduino we have in the kit.
 * Go to Tools -> Port, and you should be able to see a port name, which shows that your system recognizes the Arduino (Various OS will show up the port differently)
 * You can press the right arrow to upload your code to your Arduino. You'll see a message "Done uploading" on the bottom of the screen.
 * File -> Examples have some very well documented Arduino codes.
   * File -> Examples -> 01.Basics -> Blink  is a simple example that blinks a built-in LED
 * Arduino boards usually have a "reset" button to temporarily stop the code from running.
 * Red = power; black, brown = ground; yellow,orange,green = signal
 * PIR sensor pins to cable - conventional colors:
   * Brown - Ground
   * Red - Power ("VCC", "+5V") 
   * Yellow - "signal"
 * 
 * Accelerometer sensor pins to cable to Arduino Pin # - suggested ad hoc color convention
   * Brown - Ground
   * Red - Note!!  plug into the 3.3 Volt Pin
   * X_Out/X-Axis - Orange - Pin A0
   * Y_Out/Y-Axis - Yellow - Pin A1
   * Z-Out/Z-Axis - Green - Pin A2


Code for the accelerometer:

```
// the setup routine runs once when you press reset:
void setup() {
  // initialize serial communication at 9600 bits per second:
  Serial.begin(9600);
}

// the loop routine runs over and over again forever:
void loop() {
  // read the input on analog pin 0:
  int sensorValueX = analogRead(A0);
  int sensorValueY = analogRead(A1);
  int sensorValueZ = analogRead(A2);
  // print out the value you read:
  Serial.print(sensorValueX*5/1023.0);
  Serial.print(',');
  Serial.print(sensorValueY*5/1023.0);
  Serial.print(',');
  Serial.println(sensorValueZ*5/1023.0);
  delay(100);        // delay in between reads for stability
}
```

 * For the future: To play with  the temperature sensor (silver cylinder on the long black wire):
   * Sketch -> Include Library -> Manage Library
     * Load DallasTemperature by Miles Burton, et al.
     * Load OneWIre by Jim Studt, et al.
   * Caveat: this device needs a "pull up resistor" - not yet covered.

