Emokit
======

Reverse engineering and original code written by

* Cody Brocious (http://github.com/daeken)
* Kyle Machulis (http://github.com/qdot)

Contributions by

* Severin Lemaignan - Base C Library and mcrypt functionality
* Sharif Olorin  (http://github.com/fractalcat) - hidapi support

Description
===========

Emokit is a set of language for user space access to the raw stream
data from the Emotiv EPOC headset. Note that this will not give you
processed data (i.e. anything available in the Emo Suites in the
software), just the raw sensor data.

The C library is backed by hidapi, and should work on any platform
that hidapi also works on.

The Python library is currently very broken. Fix it!

Information
===========

FAQ (READ BEFORE FILING ISSUES): http://github.com/openyou/emokit/FAQ.md

If you have a problem not covered in the FAQ, file it as an
issue on the github project.

PLEASE DO NOT EMAIL OR OTHERWISE CONTACT THE DEVELOPERS DIRECTLY.
Seriously. I'm sick of email and random facebook friendings asking for
help. What happens on the project stays on the project.

Issues: http://github.com/openyou/emokit/issues

Required Libraries
==================

* CMake - http://www.cmake.org
* libmcrypt - https://sourceforge.net/projects/mcrypt/
* hidapi - http://www.signal11.us/oss/hidapi/

Usage
=====

C library
---------

See epocd.c example

Platform Specifics Issues
=========================

Linux
-----

Due to the way hidapi works, the linux version of emokit can run using
either hidraw calls or libusb. These will require different udev rules
for each. We've tried to cover both (as based on hidapi's example udev
file), but your mileage may vary. If you have problems, please post
them to the github issues page (http://github.com/openyou/emokit/issues).

Credits - Cody
==============

Huge thanks to everyone who donated to the fund drive that got the
hardware into my hands to build this.

Thanks to Bryan Bishop and the other guys in #hplusroadmap on Freenode
for your help and support.

And as always, thanks to my friends and family for supporting me and
suffering through my obsession of the week.

Credits - Kyle
==============

Kyle would like to thank Cody for doing the hard part. 

He would also like to thank emotiv for putting emo on the front of
everything because it's god damn hilarious. I mean, really, Emo
Suites? Saddest hotel EVER.
