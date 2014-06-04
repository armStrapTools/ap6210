ap6210
======

Wifi and Bluetooth driver for CubieTruck.

This patch should be applied to the root of the linux-sunxi kernel's source :

    # patch -p1 < ap6210_defconfig.patch
    # patch -p1 < ap6210_module.patch

To load the module, add the following line to /etc/modules :

    ap6210

Feel free to improve the code and submit bugfix...

