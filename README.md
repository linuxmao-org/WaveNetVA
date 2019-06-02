# WaveNetVA

Feedforward WaveNet for black-box virtual analog modeling. This code is related to our paper submitted to [SMC 2019](http://smc2019.uma.es/): https://link-to-pre.print

A real-time implementation of the model built using JUCE. The code can be built as a standalone audio application or as an VST3, AU or AAX etc. plugin.

Audio samples are available on the [demo page](http://research.spa.aalto.fi/publications/papers/smc19-black-box/).

## Getting Started

### Installing

These instructions are specific to a **LV2 build** realized by linuxmao.org.  
If you are interested in VST, check the [original repository](https://github.com/damskaggep/WaveNetVA).

* Clone the repo.
* Install development packages: eigen3 alsa freetype2 libcurl x11 xext xinerama libgl1-mesa xcursor xrandr
* Open a terminal and visit the build directory: `cd Builds/LinuxMakefile`
* Run the command: `make -f Makefile.LV2 CONFIG=Release`
* Copy `build/WaveNetVA.lv2` into a LV2 path of your choice.

Note that there also is a standalone version: build/WaveNetVA

### Loading trained models

The trained models are stored as json files. The pre-trained models of the Ibanez Tube Screamer, Boss DS-1 and Electro-Harmonix Big Muff Pi described in the paper are included in the [Models](Models) directory.

## License
This project is licensed under the Apache License, Version 2.0 - see the [LICENSE](LICENSE) file for details.
