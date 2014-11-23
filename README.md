NATTER
======

This is NATTER, a simple tool for all those not lovers out there!
----

+ Are you a **NAT** novice that is bored of always having the same carrier grade nat IP?

+ Or are you a **NAT** enthusiast, embracing the multiple router per line concept?

+ Maybe you are an advanced **NAT** fanatic with that special urge for scrambled and unsuperable network traffic?

NATTER is aiming to turn your life around!


Purpose
=======

**NATTER** will create close to an arbitrary number of nats on your local linux
machine. Using the unmatched performance of linux network namespaces and
netfilter **NATTER** will create a network expose that you will never forget!


Requirements
============

+ linux
+ iptables
+ ip-netns ( part of iproute2 )


Usage
=====

    sudo ./natter [-n num] [-c (A,C)] [-s] [-d]

+ Use `-n num` to create tens, hundreds or even thousands of NATs!
+ RFC 1918 private network
  - -c C for old school 192.168.0.0/24 networks ranges
  - -c A for NAT in the 10.0.0.0/8 network range, use this to fit your ambitious nating demands
+ Extra option "-s" to safely turn off the last chance of ever creating an incoming connection again by using a random IP address in each nat network!
+ Use `-d` to turn off NAT, be warned as this may expose you to the internet!


ToDo/Bugs
=========

+ Future versions will facilitate the endless capabilities of IPv6-NAT technology, stay tuned
+ Enterprise version planned, contact me privately
+ starting with 500 layers I am experiencing unexplained network drops that I cannot explain yet
+ tested on only 2 machines so far, be careful

Reference
=========

A good starting point for why **NATTER** is awesome can be found here:

[http://www.heise.de/netze/news/foren/S-Zwangsrouter-Bundesnetzagentur-verdreht-Ziel-der-grossen-Koalition-ins-Gegenteil/forum-286036/list/](http://www.heise.de/netze/news/foren/S-Zwangsrouter-Bundesnetzagentur-verdreht-Ziel-der-grossen-Koalition-ins-Gegenteil/forum-286036/list/)
