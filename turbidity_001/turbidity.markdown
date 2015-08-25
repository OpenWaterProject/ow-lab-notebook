
<img src="./assets/turbidity.png">


Just wanted to gather some useful materials around turbidity -- how it's usually assessed, and various approaches one might take to measuring it.

# Background

The gist (as far as I yet understand!) is:  measuring the amount of suspended solids in water -- solids that haven't fully dissolved --  is a commonly used water quality parameter. In many contexts, having a lot of solids floating in the water -- stuff like silt, clay, algae, other organic matter  -- is undesirable, so folks want some associated metric.  For a rough measure, we can often simply *look* at a given sample of water --  water with a lot of solids floating in it will tend to look more opaque -- it'll look 'muddy'.  But in order to really track changes over time, or compare different bodies of water, it's often nice to have a metric that is more precise than 'not very muddy' vs. 'pretty muddy'. [1] This motivates folks to define what they call 'turbidity': there are various specific definitions of turbidity, but in general they all involve an assessment of the amount of suspended solids that relies on shining light through the water, and then making optical measurements of what light emerges from the water sample.  The idea is that solid particles will tend to scatter light in revealing ways, rather than allowing it to pass through in the manner it would without any suspended matter present in the water.  

# Standards / references / definitions

Sensor approach / design depends on goals.  Various (overlapping) goals might include: 
- Data that approaches EPA standards for turbidity
- Data that indicates sudden changes in turbidity level, useful as a 'trigger' for water sampling / photo taking
- Colorimetric data that might correlate with various contaminants / types of suspended solids.

So, what are the various definitions / approaches?

Background readings / materials:

- [Fondriest review](http://www.fondriest.com/environmental-measurements/equipment/measuring-water-quality/turbidity-sensors-meters-and-methods/)
- [EPA review](http://water.epa.gov/lawsregs/rulesregs/sdwa/mdbp/upload/2001_01_12_mdbp_turbidity_chap_11.pdf)


![single](./assets/single-beam-color.png)

![multiple](./assets/four-beam-color.png)

![scatter](./assets/scatter-patterns-color.png)

![sensor-design](./assets/sensor-design.png)


# First steps towards measurement

- Chris' design for PVC housing

<img src="./assets/pvc-1.jpg" width=300>

<img src="./assets/pvc-2.jpg" width=400>

<img src="./assets/pvc-3.jpg" width=400>

"It looks like you have to measure light intensity at 90° from light direction. So you need a mirror.

The design above has two features:

- There is only one simple small window that has to be waterproofed.

- The baffle keeps ambient light to a minimum but allows plenty of water to circulate in front of the window.

Since you need to measure at 90°, you can just put a mirror on the baffle at 45°. Shoot the light straight out to it and measure it a cm from the mirror."


- Pete design

![linear1](./assets/linear-1.png)

![linear2](./assets/linear-2.png)

- sketch of design idea with Bethany re: pvc / riffle


- Hackteria.org design for DIY turibidy meter: http://hackteria.org/wiki/index.php/DIY_turbidity_meters

- 'Affordable Open-Source Turbidimeter' http://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&ved=0CCkQFjABahUKEwiagNbHtsPHAhWBbD4KHer-AF8&url=http%3A%2F%2Fwww.mdpi.com%2F1424-8220%2F14%2F4%2F7142%2Fpdf&ei=BfPbVdrpGYHZ-QHq_YP4BQ&usg=AFQjCNEaOSQL8Hzs4HLt5y-m1jHs-HROGg&sig2=LQc0_LE4zv79vbMGlUEcBw
- and: https://github.com/wash4all/open-turbidimeter-project
- supplementary material: http://www.mdpi.com/1424-8220/14/4/7142/s1

- cell concentration turbidimeter (open source ecology) http://opensourceecology.org/wiki/CellConcentrationTurbidimeter

## Sensors


- [Adafruit TSL2591 High Dynamic Range Digital Light Sensor](http://www.adafruit.com/products/1980?gclid=Cj0KEQjwgeuuBRCiwpD0hP3Cg4kBEiQAHflm1hb43Ub5CR7TSTamNBer7x-t3-FwrEZkxcEN1Hy_rXMaAlLP8P8HAQ); [tutorial](https://learn.adafruit.com/adafruit-tsl2591)

<img src="./assets/tsl2591.jpg" width=250>

Notes: this sensor seems good b/c it's sensitive in the IR as well, and the recommended wavelength for some of the turbidity sensors is in the IR.

- [GA1A12S202 Log-scale Analog Light Sensor](http://www.adafruit.com/products/1384?gclid=Cj0KEQjwgeuuBRCiwpD0hP3Cg4kBEiQAHflm1mFemOLx3eg_rCWAgsncuij1epxwds8A0sAr97IrN-0aAqib8P8HAQ)
- Craig's photocell + op-amp idea
- light-frequency converter (for Coqui-like device): http://www.ti.com/lit/ds/symlink/tsl235.pdf


# Next steps


[1] Not always, though! Depending on the question one is interested in, or the audience, it may be enough to simply to e.g. take a photo of a river and show that it looks 'pretty muddy'.  Mining operations and runoff from farmlands can turn normally-clear rivers muddy, and in some contexts this is enough to indicate a problem / trigger regulatory action.  Also: a measurement of water 'transparency', which can be related to turbidity, using a simple Secchi disk device (https://en.wikipedia.org/wiki/Secchi_disk) has for several decades been used as a very effective way to track the evolution of turbidity in various water bodies. 
