
# Ressources
Download [Firmware](http://micropython.org/download#esp8266)

# init ESP


pip install esptool
esptool.py --port /dev/ttyUSB0 erase_flash
esptool.py --port /dev/ttyUSB0 --baud 460800 write_flash --flash_size=detect 0 esp8266-20170108-v1.8.7.bin

picocom /dev/ttyUSB0 -b115200

import webrepl_setup
