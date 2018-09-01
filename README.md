# Linux Huion Config

Config files and instructions for using a Huion H1060P drawing tablet with Linux

## Dependencies

* Ubuntu >= 18.04
* Huion H1060P drawing tablet
* [digimend-kernel-drivers](https://github.com/DIGImend/digimend-kernel-drivers)

## Getting Started

* Install digiment-kernal-drivers
* Make sure to follow directions to add
`Section "InputClass"
    Identifier "Tablet"
    Driver "wacom"
    MatchDevicePath "/dev/input/event*"
    MatchUSBID "256c:006e"
EndSection`

to `/usr/share/X11/xorg.conf.d/70-wacom.conf`
* Restart computer
* Run `./xsetwacom-krita-config.sh` to set buttons to Krita shortcuts

## Resources

* [xsetwacom manual](https://www.mankier.com/1/xsetwacom)

## License

Linux Huion Config is released under the MIT License. See license.txt for more details.