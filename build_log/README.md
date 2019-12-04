# Parts list

- [Iris Rev 2 PCBs](https://keeb.io/collections/keyboard-pcbs/products/iris-keyboard-split-ergonomic-keyboard) (Only Rev 4 is available now)
- 2 Arduino Pro Micros (1 [regular](https://keeb.io/collections/frontpage/products/pro-micro-5v-16mhz-arduino-compatible-atmega32u4) and 1 [elite-c](https://keeb.io/collections/frontpage/products/elite-c-usb-c-pro-micro-replacement-arduino-compatible-atmega32u4))
- 3D-printed case
- [M3 nuts & bolts](https://www.amazon.com/gp/product/B072FKMYMF/) (for attaching the tenting legs)
- 53 "Trash Panda" key switches (purchased from someone on Reddit's [mechmarket](https://www.reddit.com/r/mechmarket/))
- Canvas Ortho Keycap set (purchased from someone on Reddit's [mechmarket](https://www.reddit.com/r/mechmarket/))
- [TRRS Cable](https://keeb.io/products/trrs-cable?variant=8139444519018)
- [Magnetic USB Cable](https://www.amazon.com/gp/product/B07QCWMQW9/)

# The case

The case was 3D printed using [these Iris case files](https://github.com/wizarddata/Iris-Case/tree/master/High%20Profile) by [wizarddata](https://github.com/wizarddata) (thanks for making these available!). The parts were printed at at the [GWU Innovation Center](https://innovation.gwu.edu/gw-innovation-center) (shout out to Konstantin Mitic for all the help with this!).

<img src="https://github.com/jhelvy/iris/raw/master/build_log/img-build/2-printed_pieces.jpg" width="600">

After printing the parts, I tried to create a "wood"-like look for the top pieces by attempting to stain them (staining plastic is tricky, but do-able). I started by coating the parts in a black stain to try and build some variation in the main color. After that dried (about 24 hours later), I coated the parts again in a stain-polyurethane blend by Midwax (I used [Olde Maple(https://www.minwax.com/wood-products/one-step-stain-and-finishes/minwax-polyshades)]). The polyurethane in the blend helped keep the color in place as it all dried.

Black stain layer | Stain-polyurethane coating
------------------|----------------------------
<img src="https://github.com/jhelvy/iris/raw/master/build_log/img-build/3-painting1.jpg" width="400"> | <img src="https://github.com/jhelvy/iris/raw/master/build_log/img-build/4-painting2.jpg" width="400">

Since the back pieces were black plastic and therefore the stain color wouldn't work, I attempted to give them a metallic look by spray painting them with a silver colored ["Hammered Spray Paint"](https://www.rustoleum.com/product-catalog/consumer-brands/universal/universal-hammered-spray-paint) by Rust-Oleum.

# Assembly

For the most part, I followed the [Iris build guide](https://docs.keeb.io/iris-rev2-build-guide/), which is pretty straight forward. However, I made one gigantic error, and one smaller error (I'll get to those in a bit).

I started by flashing the pro-micros to make sure they work, following the guide [here](https://docs.keeb.io/flashing-firmware/). Once I was confident the pro-micros were good, I moved on to soldering the diodes, TRRS jacks, and reset switches.

Here's where I made the gigantic error - I went straight to soldering the switches...big mistake. Instead, I should have soldered on the pro-micro header pins _before_ the switches. Realizing my error too late, I de-soldered the two switches that sit just over the pro-micro and had to solder the pro-micro header pins from the top side of the switch plate, which was ridiculously tedious. Once I got that error fixed, I moved on to soldering on the pro-micros.

The smaller error was adding the rotary encoder at the end. This was mostly because I decided later on to add it, but in retrospect I should have installed it prior to soldering in the switches. Having to solder it at the end left me little wiggle room when trying to get the pins all aligned and wired up. In the end, I was able to get it in place by first soldering on three wires to the three pins on the encoder then feeding those wired down through the switch plate and around the bottom of the PCB. I then soldered the two other leads on the encoder to the PCB where you would otherwise solder a key switch, and added a dab of Gorilla Glue to keep the whole thing nice and set in place. The two


