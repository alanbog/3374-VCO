# 3374-VCO

This repository contains a circuit designed to be a clone of the CEM 3374 VCO IC used in analog synthesizers from the early 1980s such as:

* Fender Chroma Polaris
* Oberheim Matrix 12
* Oberheim Xpander
* Akai VX600

It is designed to operate with 12V for Vcc and -5V or -6V for Vee, which is what all of the synthesizers listed above use for supply voltages. The circuit contains two oscillator channels with triangle and sawtooth wave outputs. Triangle wave outputs have an amplitude of 1/3 Vcc, and sawtooth wave outputs have an amplitude of 2/3 Vcc. Synthesizers using the CEM 3374 that generate square/pulse waves do so with external comparator circuits. 

Channel A sync is implemented. Channel B sync is not implemented, but this feature was rarely used on the CEM 3374 (None of the synthesizers listed above use it). 

A thermistor circuit is used to provide a temperature compensated reference voltage. Typically, this voltage is used as a reference for the DAC that outputs the voltage that controls the frequency of the oscillators.

This was tested on a Chroma Polaris. It should work in all of the other synthesizers listed above, but it hasn't been tested. 

![3374 VCOs next to a CEM 3374 IC](https://github.com/alanbog/3374-VCO/blob/master/3374%20VCO.jpg?raw=true)
