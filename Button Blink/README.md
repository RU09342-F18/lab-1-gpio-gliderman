# Nate Hoffman's Button Blink

Control of an LED state based on the state of a button.

## Operation

A while loop is used to continuously poll the state of the button. An if statement performs this check by ANDing the input port with the button's pin to determine a 1 or 0 state. A 1 state means the button is not pressed (as there is a pull-up resistor), while a 0 state means the button is pressed. Based on which state, the LED is set to a 1 for pressed or 0 if not pressed.

## Devices

Code was written to run on both an MSP430G2553 and an MSP430F5529. Both blink the LED on pin 1.0.
