# Nate Hoffman's Simple Blink

This code blinks an LED that is on a development board at a fixed rate.

## Operation

A while loop is used to continuously toggle the LED on and off. The LED is toggled by XORing with `BIT0`. A for loop then counts through 5000 times to make the processor do nothing for a period of time.

## Devices

Code was written to run on both an MSP430G2553 and an MSP430F5529. Both blink the LED on pin 1.0.
