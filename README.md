# Kernel for Samsung Galaxy Tab3 Lite (SM-T110) 

Use goyawifi_pmos_defconfig to build kernel for PostMarketOS

Original sources from http://opensource.samsung.com (SM-T110_EUR_XX T110XXUANA7)

Use goyawifi_defconfig to build a kernel for stock ROM (untouched!)
Use goyawifi_recovery_defconfig to build a kernel for custom recovery (w/SELinux|NoBootLoop)

Using GCC4.7

https://askubuntu.com/questions/1235819/ubuntu-20-04-gcc-version-lower-than-gcc-7

```
sudo apt-get install gcc-4.7 gcc-4.7-arm-linux-gnueabi-base gcc-4.7-arm-linux-gnueabi gcc-4.7-arm-linux-gnueabihf-base \
	gcc-4.7-arm-linux-gnueabihf-base gcc-4.7-base gcc-4.7-multilib-arm-linux-gnueabi \
	gcc-4.7-multilib-arm-linux-gnueabihf libgcc-4.7-dev-armel-cross libgcc-4.7-dev-armhf-cross \
	libgcc-4.7-dev libhfgcc-4.7-dev-armel-cross libsfgcc-4.7-dev-armhf-cross

sudo apt-get install g++-4.7
```

Building for pmOS:

```
make goyawifi_pmos_defconfig

make -j4

```