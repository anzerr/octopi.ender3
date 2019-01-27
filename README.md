
### `Intro`
Wanted to use Octoprint on a raspberry pi zero w as it's small footprint and low power usage.

Warning: The zero w will not work with a camera the CPU usage is to hight negatively impacting printing results

### `Bill of materials`

- 1 x Boost Buck Converter XL6009
- 2 x T Block Square nuts 2020 m3 or printed version // https://www.thingiverse.com/thing:3050607
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
- Hot glue
- 1 x usb mini B to usb

### `Setup Pi`
- Download the os https://octoprint.org/download/
- Use etch flash the image onto a sd card (https://github.com/balena-io/etcher)
- edit octopi-wpa-supplicant.txt to with your wifi credenciales

### `Prints`
You can print most of these without supports

- 1 x xt60_y_connector (no support)
- 1 x pi_base (no support)
- 1 x boost_base (no support)
- 1 x case (touching buildplate support)
- 2 x spacer_pi (touching buildplate support)
- 1 x spacer (no support)

There should be no clean up needed. Add the two brass inserts to the pi_base

### `Wiring`
- Creating the xt60 Y connector.
- Use the left over male connector with the 14awg cable to create wiring to the buck converter.
- Set the buck converter to a little under 5v
- Wire power to the pads under the raspberry pi
- Cut the male usb mini b cable to length and strip
- add the 1k ohm resistor between the +5v on the pi and the red wire from the usb mini
- wire the rest, black to gnd, green to d+ and white to d-. (on my usb mini cable I had to swap d+ and d-)

### `Images`