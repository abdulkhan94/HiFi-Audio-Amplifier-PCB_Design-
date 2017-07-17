# Transparent HiFi Audio Amplifier for Headphones
## Introduction
The goal of our Transparent HiFi USB Audio Amplifier system is to take in a audio signal via USB, allow the user to modify amplifier and volume controls, and to hear the modified audio signal through headphones. Our system specifications are for our design to not produce a DC offset that’s greater than 20mV, to not produce excessive power spikes greater than 50mV, have an output impedance of less than 2 ohms, and to support 8 specific headphones with a range of impedances from 16 to 600 ohms. The left and right audio signals must have flat frequency responses (+/-2.5dB), linear/flat phase responses without being set at 0dB, noise under -105dBv (-103dBu) and distortion under 1% THd into 150 ohms at 1Vrms. Lastly, the power amplifier must have a slew of under 3V/us by a square wave of 600 ohms. 

## Power Amplifier
The power amplifier subsystem will get a 1 V pk-pk signal input from the Amplifier controls subsystem and will amplify that to output analog audio signal across various headphones. All parts of the subsystem will be powered by +13/-13 DC Voltage signal. The subsystem consists of two different parts to achieve amplification of both current and voltage.
The first stage of the design consists of a preamplifier design. This is essentially a Class A audio amplifier which is implemented in order to boost the voltage of the 1 V pk-pk signal that the subsystem receives as input from the amplifier controls subsystem. A major design consideration that has been made here revolves around amplifying voltage to the adequate level while maintaining low noise in the signal. The design consists of two biasing resistors followed by a NPN transistor. This part of the design is powered by a +13V DC power rail. 
The next step of the design consists of the power amplifier which amplifies the current. This part of the subsystem is required to have enough current in order to drive the output across the headphones. A class AB amplifier design has been implemented here in order to achieve the adequate current amplification. This design also consists of two biasing resistors for each transistor and is powered by +/- 13V DC power rails.

## Current Status
* All subsytems of the design have been finalised and layed out on PCB's. 
* All subsystems integrated and fully functional.
