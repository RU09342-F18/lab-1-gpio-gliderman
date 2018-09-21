# Nate Hoffman's Multiple Blink

This code blinks two LEDs on a devlopment board at separate rates. For each full cycle of one LED (on and then off), the other LED cycles 5 times.

## Operation

A while loop is used to continuously change the states of the LEDs. The first step is to toggle the first LED. Then, a for loop nested in the while loop runs five times with two parts. The first part toggles the state of the second LED, and the second part is a for loop that loops 10000 times to delay the processor from moving to the next iteration of the main for loop.

## Devices

Code was written to run on both an MSP430G2553 and an MSP430F5529.
