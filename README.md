# Nokia 3210 Retrofit Board Aplications

This repository contains files for applications to support i.MX7 Nokia 3210 Mainboard

## System requirements
In addition to the required packages given by the android source.android.com/source/initializing.html these packages are needed as well:

	$ sudo apt install uuid uuid-dev
	$ sudo apt install zlib1g-dev liblz-dev
	$ sudo apt install liblzo2-2 liblzo2-dev
	$ sudo apt install lzop
	$ sudo apt install git-core curl
	$ sudo apt install u-boot-tools
	$ sudo apt install mtd-utils
	$ sudo apt install android-tools-fsutils
	$ sudo apt install openjdk-8-jdk

## Get build environment

	$ mkdir android
	$ cd android
	$ repo init -u https://android.googlesource.com/platform/manifest -b android-7.1.1_r13
	$ repo sync

Cloning into Android will download 100+ different git repositores. So it will take some time.

	$ git clone git://git.freescale.com/imx/linux-imx.git kernel_imx
	$ cd kernel_imx
	$ git checkout n7.1.1_1.0.0-ga

Cloning into the imx Kernel will take some time as well

	$ cd ..
	$ cd bootable
	$ mkdir bootloader
	$ cd bootloader
	$ git clone git://git.freescale.com/imx/uboot-imx.git uboot-imx
	$ cd uboot-imx
	$ git checkout n7.1.1_1.0.0-ga


