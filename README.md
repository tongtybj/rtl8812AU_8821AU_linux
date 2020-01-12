
1;4205;0c# rtl8812au

Realtek 8812AU/8821AU USB WiFi driver.

## Compiling with DKMS

Clean the system from previous drivers if any and clone current repository

```sh
# sudo apt purge rtl8812au-dkms
# sudo apt install git
# git clone https://github.com/tongtybj/rtl8812AU_8821AU_linux.git
# cd rtl8812AU_8821AU_linux
```

Install kernel headers 

```sh
# sudo apt install linux-headers-$(uname -r)
```

Install support for WiFi adapter

```sh
# sudo make -f Makefile.dkms install
# sudo modprobe rtl8812au
```
