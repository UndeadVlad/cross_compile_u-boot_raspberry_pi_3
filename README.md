# cross_compile_u-boot_raspberry_pi_3

## **Установка необходимых пакетов для компиляции u-boot**
  * `sudo apt-get install gcc-aarch64-linux-gnu`
  * `sudo apt-get install device-tree-compiler`
  
## Скачаем и распакуем исходные коды последней версии U-Boot:
  * `wget ftp://ftp.denx.de/pub/u-boot/u-boot-latest.tar.bz2`
  * `tar -jxf u-boot-latest.tar.bz2`

## Сборка u-boot
  * `make CROSS_COMPILE=aarch64-linux-gnu- clean`
  * `make CROSS_COMPILE=aarch64-linux-gnu- distclean`
  * `make CROSS_COMPILE=aarch64-linux-gnu- rpi_3_defconfig`
  * `make CROSS_COMPILE=aarch64-linux-gnu-`

### Файлы defconfig для разных Raspberry Pi
  * `rpi_defconfig`       - For Raspberry pi A, A+, B, B+
  * `rpi_2_defconfig`     - For Raspberry pi 2 board
  * `rpi_3_defconfig`     - For Raspberry pi 3 board
  * `rpi_3_32b_defconfig` - For Raspberry pi 3 32 bit u-boot
