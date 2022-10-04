# SonoffEspressoTimer
This is a Coffee Machine Controller with a Sonoff Basic as a Timer. This project doesn't attempt to create a PID for any Espresso machine, but be the simplest single- & double-shot timer that can be integrated.

## Setup
Connect the Pump of the Coffee Machine to the Output of the Sonoff and the Pushbutton to GPIO 14 and Ground.
Connect TX to SCK and RX to SDA of the Display. (0,96" OLED)


## Usage
The Controller tries to connect to specified WiFi. Just set up your local Wifi in Code before flashing the Sonoff.
You can connect to the Sonoff by typing "SonoffEspresso/" or the IP in your Webbrowser.
The Webinterface is presented to programm the pumping Time for single and double Shot.

There are 3 Operation-Modes:
- Single: Brewing for the Time you set for Singleshot
- Double: Brewing for the Time you set for Doubleshot
- Manual: Brewing as long as the Button is held

If you push the button again while the machine is brewing the machine will stop.

Saving new Times:
- Start Single- or Doubleshot brweing
- Push the Button again and hold as long as you want
- New brewing Time is saved for Single- or Doubleshot


This project is a modificatin of ljans sonoffgrinder https://github.com/ljan/sonoffgrinder
Thanks to timo.helfer @ www.kaffeenetz.de for the inspiration and codebase.
