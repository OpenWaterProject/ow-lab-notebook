
<img src="./assets/turbidity.png">


Just wanted to gather some useful materials around turbidity -- how it's usually assessed, and various approaches one might take to measuring it.

# Background

The gist (as far as I yet understand!) is:  measuring the amount of suspended solids in water -- solids that haven't fully dissolved --  is a commonly used water quality parameter. In many contexts, having a lot of solids floating in the water -- stuff like silt, clay, algae, other organic matter  -- is undesirable, so folks want some associated metric.  For a rough measure, we can often simply *look* at a given sample of water --  water with a lot of solids floating in it will tend to look more opaque -- it'll look 'muddy'.  But in order to really track changes over time, or compare different bodies of water, it's often nice to have a metric that is more precise than 'not very muddy' vs. 'pretty muddy'. [1] This motivates folks to define what they call 'turbidity': there are various specific definitions of turbidity, but in general they all involve an assessment of the amount of suspended solids that relies on shining light through the water, and then making optical measurements of what light emerges from the water sample.  The idea is that solid particles will tend to scatter light in revealing ways, rather than allowing it to pass through in the manner it would without any suspended matter present in the water.  

# Standards / references / definitions

- EPA
- Sensor approaches
- Secchi disk
- 'Trigger' ideas.

So, what are the various definitions?


- http://www.fondriest.com/environmental-measurements/equipment/measuring-water-quality/turbidity-sensors-meters-and-methods/


# First steps towards measurement

- Chris design
- Pete design
- Adafruit sensors
- sketch of design idea with Bethany re: pvc / riffle 

# Next steps


[1] Not always, though! Depending on the question one is interested in, or the audience, it may be enough to simply to e.g. take a photo of a river and show that it looks 'pretty muddy'.  Mining operations and runoff from farmlands can turn normally-clear rivers muddy, and in some contexts this is enough to indicate a problem / trigger regulatory action.  Also: a measurement of water 'transparency', which can be related to turbidity, using a simple Secchi disk device (https://en.wikipedia.org/wiki/Secchi_disk) has for several decades been used as a very effective way to track the evolution of turbidity in various water bodies. 
