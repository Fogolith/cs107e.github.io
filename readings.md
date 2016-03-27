---
layout: page
title: Resources
permalink: /resources/
---

### Raspberry Pi Hardware

We are using the Raspberry Pi A+ in class. The A+ is similar to the B+.

* [Raspberry Pi Board Schematics](https://github.com/raspberrypi/documentation/blob/master/hardware/raspberrypi/schematics/README.md)

### ARM

The Raspberry Pi A+ uses a Broadcom BCM2835 chip. 
Inside the chip is an ARM1176JFZ-S processor 
which is based on the ARMv6 architecture.

* [Broadcom BCM2835 Peripherals Documentation](../readings/BCM2835-ARM-Peripherals.pdf )

  * [Errata](http://elinux.org/BCM2835_datasheet_errata)

  * [GPIO Pad Control](http://www.scribd.com/doc/101830961/GPIO-Pads-Control2).

* The ARM1176JFZ-S processor is documented in the 
[Technical Reference Manual](http://infocenter.arm.com/help/topic/com.arm.doc.ddi0301h/DDI0301H_arm1176jzfs_r0p7_trm.pdf).  

* ARM1176JFZ-S processors use the ARMv6 architecture,
which is documented in [ARMv6 Architecture Manual](../readings/armv6.pdf).
The following [excerpt](../readings/armisa.pdf)
describes just the instructions.

* ARM System Developer's Guide: Designing and Optimizing System Software (The Morgan Kaufmann Series in Computer Architecture and Design), Andrew Sloss, Dominic Symes, and Chris Wright, 2004. This book is a bit dated, but still provides an excellent overview of low-level ARM programming.

* Excellent [slides](http://twins.ee.nctu.edu.tw/courses/ip_core_02/handout_pdf/Chapter_2.pdf) by Prof. Yen at NCTU on the ARM processor core and instruction sets.

### ARM Assembly Language

* Carl Burch's [Introduction to ARM Assembly Language](http://www.toves.org/books/arm/) is highly recommended starting point.

* [Worldwind Tour of ARM Assembly](http://www.coranac.com/tonc/text/asm.htm) from the TONC Guide to programming the Nintendo Game Boy Advance (which uses am ARM processor).

* [Davespace Introduction to ARM Course](http://www.davespace.co.uk/arm/introduction-to-arm/index.html).

* [Thinkingeek ARM Assembler for the Raspberry Pi](http://thinkingeek.com/2013/01/09/arm-assembler-raspberry-pi-chapter-1/).

### Bare Metal Programming

* David Welch's excellent set of [bare metal programming examples](https://github.com/dwelch67/raspberrypi).

* Steve Halliday's [videos](http://computersciencevideos.org/Raspberry-Pi/Raspberry-Pi-Setup) about programming the raspberry pi.

* Alex Chadwick's [Baking Pi Course](http://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/os/).

* The [Raspberry Pi Bare Metal Forum](http://www.raspberrypi.org/forums/viewforum.php?f=72) has lots of information from experienced developers. Venturing into the forum is a great way to learn advanced techniques. 

### C Pogramming Language

* [EssentialC](http://cslibrary.stanford.edu/101)

* *The C Programming Language, 2nd Ed.*, B. Kernighan and D. Ritchie.
A digital copy of K&R is available to Stanford students via 
[Safari Books Online]
(http://proquest.safaribooksonline.com.ezproxy.stanford.edu/book/programming/c/9780133086249).

* *The Definitive Guide to GCC, 2nd Ed.*, William von Hagen, Apress, 2006
[pdf]
(http://sensperiodit.files.wordpress.com/2011/04/hagen-the-definitive-guide-to-gcc-2e-apress-2006.pdf)

