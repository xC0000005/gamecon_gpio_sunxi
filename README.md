gamecon_gpio_rpi
==============
gamecon_gpio_sunxi is a Linux kernel module derived from gamecon_gpio_rpi which allows interfacing various retro gamepads with Allwinner SOC GPIOs. See [wikipage](https://github.com/RetroPie/RetroPie-Setup/wiki/GPIO-Modules#gamecon_gpio_rpi) for further details.

Building dkms package on RPi
---------------------------------------------------
1. Install kernel headers
2. Copy gamecon_gpio_sunxi-\<VERSION> folder to /usr/src/
3. dkms add gamecon_gpio_sunxi/\<VERSION>
4. dkms build gamecon_gpio_sunxi/\<VERSION>
5. dkms mkdeb gamecon_gpio_sunxi/\<VERSION> --source-only
