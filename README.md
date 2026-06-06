Installation Steps:

1. Connect the ESP32-S3 to your computer using a USB cable.

2. Open Google Chrome.

3. Open the ESPTool Web Flasher: https://espressif.github.io/esptool-js/

4. Click "Connect".

5. Select the correct COM port for your ESP32-S3.

6. Click "Erase Flash".
(This step is highly recommended because it removes old firmware, partition tables, and flash configurations that could prevent the firmware from booting correctly.)

7. After the erase process finishes, select the firmware file: Bruce-esp32-s3-st7735.bin
* located in: bruce-firmware/Bruce-esp32-s3-st7735.bin

8. Configure the flashing parameters exactly as follows:
* Address: 0x0
* Flash Mode: DIO
* Flash Frequency: 40M
* Flash Size: 16 MB

9. Click "Program".

10. Wait for the flashing process to complete.

11. After the upload finishes, the ESP32-S3 may not automatically reboot. If that happens, simply disconnect and reconnect power, or press the RESET button.

12. The Bruce Firmware should now start normally.
