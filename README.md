# keyboard

Layouts for keyboards I use.

## Ergodox Infinity

Use the [I:C Configurator](https://kiibohd.github.io/wiki/#/) to import the
JSON file. Check that `dfu-util` is installed and that `dfu-util -l` shows the
keyboard correctly when in flash mode. If not, then a udev rule is probably
missing.

```
# /etc/udev/rules.d/99-dfu.rules
SUBSYSTEMS=="usb", ATTRS{idVendor}=="1c11", ATTRS{idProduct}=="b007", GROUP="plugdev", MODE="0666"
```
