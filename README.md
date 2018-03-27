CH55x USB MIDI
----------

A repository contains WinChipHead's CH55x series MCU firmware about USB-MIDI Protocol.


TODO
----------

Implement an USB MIDI to Serial MIDI bridge properly (CH551).

Implement a Serial MIDI to USB MIDI Host bridge properly (CH554).

Implement an USB MIDI controller, for example, USB Keyboard or USB E-Drum (CH551?).

Status
----------

I have implement a loopback USB MIDI device in src directory.

BUILD
----------

You should have SDCC and my [librech551](https://github.com/rgwan/librech551) installed in your system first.

Then, Type `make` in `src/usb_device_loopback` directory will generate executable firmware binary file.

If you want to flash it to your chip, make sure that your chip is in ISP mode, blank chip will enter ISP mode automatically. If your chip has already flashed, you may have to pull-up CH55x's D+ pin, and power it up, it will enter ISP mode.

When your chip is in ISP mode, you can type `make flash` to flash firmware to your chip.

LICENSE
----------

MIT

AUTHOR
----------

Zhiyuan Wan <h@iloli.bid>
