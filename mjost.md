# README

## BUILD

To build:

```
sudo apt install avrdude avr-libc
```

```

# compile
make clean
make all
make flash


# upload
avrdude -c arduino -P /dev/ttyUSB0 -p atmega328p -B 10 -F -U flash:w:grbl.hex:i
```

## CONNECTIONS

### PROBES

BOARD PROBE => AD4 instead of original AD5 (i.e. uC pin 4 instead of originall pin 5)
TOOL PROBE  => GND

