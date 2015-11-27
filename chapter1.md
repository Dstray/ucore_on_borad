# Chapter 1: Fetch Sources

## U-Boot
U-Boot is an open source Universal Boot Loader that is frequently used in the Linux community. Xilinx provides a Git tree [here](https://github.com/Xilinx/u-boot-xlnx), which can be built to accommodate different environment. After compiled to a uImage, μcore can be loaded by U-Boot.

## [Zynq Release](http://www.wiki.xilinx.com/Zynq+Releases)
Actually U-Boot is just Second Stage Boot Loader (SSBL), and the First Stage Boot Loader (FSBL) is requiered before it. Zynq Release contains pre-build FSBL, U-Boot, Linux and Device-tree Generator, which can be used to generate the boot.bin file.  
**Note** that the FSBL here could only be used on Zynq devices. For use on other board, specified FSBL sources are needed or can be built in the way described [here](http://www.wiki.xilinx.com/Build+FSBL).