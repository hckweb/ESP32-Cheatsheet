# ESP32 Cheatsheet
### Writing Flash
#### Single Writing Flash
```cmd
.\esptool.exe --port COM23 write_flash 0x00000 flash_ok_empty.bin
```
#### Multiple Writing Flash
```cmd
.\esptool.exe --port COM23 write_flash 0x10000 firmware.bin 0x910000 spiffs.bin
```
### Reading Flash
```cmd
.\esptool.exe -p COM23 -b 460800 read_flash 0 0x1000000 flash_ok_empty.bin
```
