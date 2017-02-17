# Blinker
This examples consist of two part. A transmitter (TX) and a receiver (RX).

TX will transmit a single byte LoRa packet every 200 ms.
Settings:
* SF7
* 14dBm
* 869.1MHz
* CR 4/5
* BW 125kHz

RX will listen on the same channel with the same parameters. When RX receives a packet it will toggle its LED.

This example is useful to test the range of point-to-point LoRa. When the two devices are in range you will see a flashing LED on the RX node. When the devices go out of range the LED will stop flashing.

Note that this example only test the link in one direction. For a proper experiment you will need to test in both directions.

# Hardware
This code was written for an RN2483 module connected to an Arduino Uno. Instructions on how to build this yourself are documented at: https://www.thethingsnetwork.org/forum/t/how-to-build-your-first-ttn-node-arduino-rn2483/1574
