Today Laura Perovich led Joe Goldbeck and I on an expedition to the Charles River to deploy a temperature sensor prototype.  The motivation: to test some custom temperature sensor boards that Laura had made with the intention of acquiring temperature readings that were more responsive to rapid temperature changes than a typical thermistor. We don't really know what 'fast enough' is going to be for e.g. the thermal fishing bob; but getting to know the options / range of response times for some common temperature sensors seems like a very useful exercise, in any case. The 10K thermistor we've been using on the Riffle and on the thermal fishing bob seems to be on the 'slow' side of response time: if I recall, it took about 20 seconds to register the difference between room temperature and freezing.  Several devices out there -- integrated circuits for measuring temperature, thermocouples -- have response times closer to 1 second for such a temperature difference, and some of them are potentially much easire to use and keep calibrated in the field. Additionally, digital sensors can make it easy to construct a 'chain' of sensors on a 'bus' wire, to get temperature measurements at various depths / locations simulataneously with fewer wires.  

# Laura's sensor development

Laura's previous research note on making a custom temperature sensor board is [here](http://publiclab.org/notes/lperovich/07-07-2015/thermal-fishing-bob-faster-waterproofed-temperature-sensors). 

The device she settled on was the Atmel AT30TS750A.  She


# Useful additional info

- A [comparison](http://www.ti.com/lit/an/snia009/snia009.pdf) of thermistors and integrated chip sensors; where each is useful.  

- [Thermocouple response times.](http://www.omega.com/temperature/Z/ThermocoupleResponseTime.html)

- [Thermistor performance](http://www.teamwavelength.com/info/thermistors.php)

- Edward Mallon's great writeup of [calibrating DS18B20 sensors](https://edwardmallon.wordpress.com/2015/03/30/using-ds18b20-one-wire-sensors-to-make-a-diy-thermistor-string-pt-2-calibration/)



