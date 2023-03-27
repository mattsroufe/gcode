# gcode

## Dependencies
```
brew install avrdude
python -m pip install pyserial
```

### Flash GRBL to Arduino Nano
```
avrdude -c arduino -b 57600 -P /dev/tty.usbserial-1410 -p atmega328p -vv -U flash:w:/Users/mattsroufe/Downloads/grbl_v1.1h.20190825.hex
```

### Stream Gcode
python stream.py square.ngc /dev/tty.usbserial-1410

