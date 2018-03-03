# AR150 GPS Time Source - Now supporting chrony, ntpd, and PTP!

This is my for of the lede git repo at https://github.com/lede-project/source
and contains all my changes for the AR150's time source code. its virtually the
same as the openwrt mainline fork, but in /etc/taki theres a file called lede
rather than openwrt.

All you need to is:

1. cp ar150-pps-gps-ptp.config .config
2. ./scripts/feeds update -a
3. ./scripts/feeds install -a
4. make menuconfig
5. make

and your firmware should build into: bin/targets/ar71xx/generic/openwrt-ar71xx-generic-gl-ar150-squashfs-sysupgrade.bin

Has many utilities revolving around time, network and that sort of thing.
