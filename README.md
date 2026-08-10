# This is a modified version that add IT8785 chip support. 
## I don't found any IT8785 chip datasheet and I try the driver with a Sharevdi F17h-5th industrial pc board with [success](https://github.com/bigjohnson/libgpiod-instructions-for-some-industrial-pc/tree/main/Sharevdi%20F17H-5th).

# moxa-it87-gpio-driver

https://github.com/torvalds/linux/blob/v5.2/drivers/gpio/gpio-it87.c

## Install required packages

make, linux-headers-\<KERNEL_RELEASE>

```bash
apt install --no-install-recommends -qqy make
apt install --no-install-recommends -qqy linux-headers-$(uname -r)
```

## Build package

1. Run `make` to build kernel module
2. Once build successful, `gpio-it87.ko` could be found under current directory
