# TinyOS Cooja Simulator
This is a TinyOS application which transfer data between three motes and according to the seder ID turn off/on the LEDs.
In this application there are three files called "RadioCountToLeds.h", "RadioCountToLedsC.nc" and "RadioCountToLedsappc.nc. 
In the header file I define the structure of the message and the message is composed by a SenderId and a counter. We have three sensors. These sensors broadcast messages. When a sensor receive a message, it turns LEDs on and off according to counters that it received. So every time a timer fires it sends a message containing this counter and sensor ID which is declared in “.h” file.
In “RadioCountToLedsC.nc” there are three timers with three different times (Milisec), and the other related interfaces including LED, boot, timer, receiving, sending, starting the radio and managing packets.

# Cooja Simulator
`cooja` is a simulator for tinyos that has GUI and you can see a snapshot of it on the below picture.
![picture](Cooja.png)
![picture](CoojaSimulation.PNG)

