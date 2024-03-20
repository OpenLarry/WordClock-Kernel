# WordClock Kernel

This is the WordClock Linux kernel, which is build using the [WordClock Buildroot](https://github.com/OpenLarry/WordClock-Buildroot) image generator.

## Changes

* Adjusted device tree in order to drive WS2812B LEDs using the LCD controller of the NXP i.MX233 processor (inspired by [SpritesMods](https://spritesmods.com/?art=imx233-ws2811)).
* Added VSync support to the LCD framebuffer driver.
* Fixed scale issues with the LRADC IIO driver.

## Linux kernel

There are several guides for kernel developers and users. These guides can
be rendered in a number of formats, like HTML and PDF. Please read
Documentation/admin-guide/README.rst first.

In order to build the documentation, use ``make htmldocs`` or
``make pdfdocs``.  The formatted documentation can also be read online at:

    https://www.kernel.org/doc/html/latest/

There are various text files in the Documentation/ subdirectory,
several of them using the Restructured Text markup notation.
See Documentation/00-INDEX for a list of what is contained in each file.

Please read the Documentation/process/changes.rst file, as it contains the
requirements for building and running the kernel, and information about
the problems which may result by upgrading your kernel.
