# arduino-menudriver
****NOTE: This git is incomplete and a work in progress. I'm in the process of tidying up my code, designing some connection diagram graphics, and producing a bare bones plug/play code snippet to make it easier for those starting out with Arduino. I'll remove this note when I feel the git is ready.*** 

A basic 4 button controlled menu demo for Arduino Uno / 1602LCD via I2C. 
by Brad Rogers - 8th March 2021. 

The purpose of this code is to rapidly implement a menu driven interface on the Arduino Uno. All the groundwork has been laid for a 2 button scroll, 2 softkey (or ok/back) interface with the ability to intercept concurrent keypresses (ie, hold left/right to access a secret menu, etc). For simplicity's sake, we'll be using a 1602 LCD driven by an i2c controller. These are super common and can be had for a couple dollars on AliExpress. Seeing as we're using the LiquidCrystal_I2C library, adapting the code to work on other displays should be a walk in the park. I'll upload such an example if I find myself needing a different display in my projects. 

We've also designed sound routines to drive both a basic single tone buzzer with a DC voltage, and also oscillations to a loudspeaker hooked up to a pin via a 100 ohm resistor for more detailed sounds. This is entrirely optional and you can choose to scrub the sound code out in your project, but from a user experience point of view, a nice reassuring beep, or encouraging/discouraging tone upon entering a function is always a nice touch. 

Hardware needed: 1602LCD with I2C adaptor, arduino uno, loudspeaker connected with a 100 ohm resistor (optional), single tone buzzer (optional), LED with 330 ohm resistor. 

I've inlcuded a demo file to showcase how we'll use the code in projects. 
