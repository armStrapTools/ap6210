ap6210
======

Wifi and Bluetooth driver for CubieTruck.

This patch should be applied to the root of the linux-sunxi kernel's source :

    # patch -p1 < ap6210_defconfig.patch
    # patch -p1 < ap6210_module.patch

The driver use GPIO 2 as the IRQ for host wakeup, this need to be setup in script.bin. Add theses lines to the board's fex and generate a new script.bin (fex2bin cubietruck.fex script.bin)

    [gpio_para]
    gpio_used = 1
    gpio_num = 2
    gpio_pin_1 = port:PH20<1><default><default><1>
    gpio_pin_2 = port:PH10<0><default><default><0>

To load the module, add the following line to /etc/modules :

    ap6210

Feel free to improve the code and submit bugfix...

