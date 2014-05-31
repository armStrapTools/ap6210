ap6210
======

Wifi and Bluetooth driver for CubieTruck.

This patch should be applied to the root of the linux-sunxi kernel's source :

    # patch -p1 < linux-sunxi-ap6210.diff

To load the module, add the following lines to /etc/modules

    ap6210_gpio_wifi
    ap6210_gpio_bt
    ap6210

Feel free to improve the code and submit bugfix...

