# Nate Hoffman's Off Board Blink

This code blinks two LEDs on a breadboard at separate rates. For each full cycle of one LED (on and then off), the other LED cycles 5 times.

## Operation

The operation mirrored the multiple blink project for the MSP430G2553.

A while loop is used to continuously change the states of the LEDs. The first step is to toggle the first LED. Then, a for loop nested in the while loop runs five times with two parts. The first part toggles the state of the second LED, and the second part is a for loop that loops 10000 times to delay the processor from moving to the next iteration of the main for loop.

## Demonstration

<blockquote class="imgur-embed-pub" lang="en" data-id="a/PQuKUKN"><a href="//imgur.com/a/PQuKUKN">Off Board Blink Demo</a></blockquote>

## Devices

This code only runs on the MSP430G2553 as that chip was able to be removed from the development board to be used in a breadboard with other supporting circuitry. Power was supplied to the chip by the development board (jumpers from the 3.3V and GND pins), and a reset button circuit was attached. Two LEDs (one red, one green) were used to demonstrate the multiple blink program.
