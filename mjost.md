# README

To build:
```
sudo apt install avrdude avr-libc
```

make clean
make all
make flash


avrdude -c arduino -P /dev/ttyUSB0 -p atmega328p -B 10 -F -U flash:w:grbl.hex:i
