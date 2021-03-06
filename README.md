
### `Intro`
Wanted to use Octoprint on a raspberry pi zero w because of its small footprint and low power usage.

Warning: The zero w will not work with a camera the CPU usage is hight negatively impacting printing results.

### `Bill of materials`
- 1 x Boost Buck Converter XL6009
- 2 x T Block Square nuts 2020 m3 or [printed version](https://www.thingiverse.com/thing:3050607)
- 1 x raspberry pi zero w
- 1 x 16gb sd card
- 2 x xt60 plug pair
- 30cm+ 14awg silicone cable
- 1 x 1k ohm resistor
- 2 x M3 Brass knurled female thread insert
- 4 x 19mm M3 screw
- 1 x 5mm M3 screw
- 1 x M3 nut
- 2 x zip ties
- Heat shrink tubing
- Hot glue or double sided tape (for the xt60 y connector)
- 1 x usb mini B to usb

### `Setup Pi`
- [Download the os](https://octoprint.org/download/)
- [Use etch flash the image onto a sd card](https://github.com/balena-io/etcher)
- Edit the octopi-wpa-supplicant.txt with your wifi credenciales.
- Connect to the octopi and finish the setup process.

### `Prints`
You can print most of these without supports. The models can be found in "./models" the source files are there with the stl. The models where made with sketchup

- 1 x [xt60_y_connector (no support)](https://github.com/anzerr/octopi.ender3/blob/master/models/stl/xt60_y_connector.stl)
- 1 x [pi_base (no support)](https://github.com/anzerr/octopi.ender3/blob/master/models/stl/pi_base.stl)
- 1 x [boost_base (no support)](https://github.com/anzerr/octopi.ender3/blob/master/models/stl/boost_base.stl)
- 1 x [case (touching buildplate support)](https://github.com/anzerr/octopi.ender3/blob/master/models/stl/case.stl)
- 2 x [spacer_pi (touching buildplate support)](https://github.com/anzerr/octopi.ender3/blob/master/models/stl/spacer_pi.stl)
- 1 x [spacer (no support)](https://github.com/anzerr/octopi.ender3/blob/master/models/stl/spacer.stl)

The only clean up needed should be drilling the holes so the screw can move freely. Add the two brass inserts to the pi_base and the parts will be ready to be assembled.

### `Wiring`
The pi pads with labels
<div style="text-align:center">
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/pads.jpg" alt="drawing" width="300"/>
</div>

- Creating the xt60 Y connector.
- Use the left over male connector with the 14awg cable to create the wiring to the buck converter.
- Set the buck converter to a little under 5v.
- Wire power to the pads under the raspberry pi.
- Cut the male usb mini b cable to length and strip.
- add the 1k ohm resistor between the +5v on the pi and the red wire from the usb mini.
- wire the rest, black to gnd, green to d+ and white to d-. (on my usb mini cable I had to swap d+ and d-)

### `Images`
<div style="text-align:center">
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/octopi_case.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/pi_side.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/octopi_nocase.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/xt60_back.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/pi_front.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/xt60_front.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/pi_side2.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/xt60_connected.jpg" alt="drawing" style="float:left" height="300"/>
	<img src="https://github.com/anzerr/octopi.ender3/raw/master/image/pi_wiring.jpg" alt="drawing" style="float:left" height="300"/>
	<span style="height:300px;float:left;width:168.75px;background:#f3f4f4;"/>
</div>