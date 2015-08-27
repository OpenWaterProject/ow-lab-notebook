A first pass on notes re: various options for broadcasting data from point to point.

The goal here is to have hardware that allows for reliable transmission of data over a distance without requiring actual cables between devices, in particular for wireless monitoring of environmental parameters.

There is a wide array of hardware approaches; we'll often use 'radio' to refer to any hardware that accomplishes wireless transmission.  Different radios are able to transmit different differences reliably for a given amount of energy (depending on the radio wavelength, and the specifics of the radio design); so energy considerations come in quickly if e.g. we're running the device off a battery. A basic list of considerations might then be:

- How far do we need to transmit? (what range should the radio have)
- Are we using a battery, or are we connected to the electrical grid? (what are the energy resources available)

If, for example, we're hoping to put a wireless node out in a field where there is no power line, and want to send information back to a base station that is 1 kilometer away, all for under $100, we'll select a radio that has at least a 1 km range when given sufficient power; and then, when we figure out what size battery + solar panel we can buy with our remaining budget, we'll have to figure out how often we can broadcast data without completely sapping the batteries before they can be recharged by the sun.

In other words -- there's some figuring involved!

So, let's take a first pass at this problem, using a particular example:  sending water parameter data from a field site to a base station.  

Here are some low-cost radios that are easy to source:

- Cell modem: Adafruit FONA (SIM800)
- 433 MHz: Moteino (RFM69)
- Bluetooth (BLE): Bluefruit (Bluetooth BLE)
- Wifi: Adafruit Wifi Module (CC3000) 

Here are some of the characteristics / pros / cons of each.

**Cell modem**.  

- [Adafruit FONA](http://www.adafruit.com/products/1963?gclid=Cj0KEQjw6vquBRCow62uo-_J_YYBEiQAMO6HimQOlkuzxVL-0okhQbUoONyUpwh6gntl6Kk8GkTCLVEaAn088P8HAQ)

<img src="./assets/fona.png" width=300>


**433 MHz**.

- [Moteino](http://lowpowerlab.com/moteino/)


**Bluetooth**.

- [nRF8001 Bluetooth LE breakout](http://www.adafruit.com/products/1697)

- [Bluefruit](http://www.adafruit.com/product/1588)

**WIFI**. 

- [Adafruit WIFI module (CC3000-based)](http://www.adafruit.com/product/1469)




 
