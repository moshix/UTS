[![Discord](https://img.shields.io/discord/423767742546575361.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/vpEv3HJ)
<a href=" https://github.com/moshix/mvs/blob/master/codenotary.com"><img src="https://raw.githubusercontent.com/moshix/mvs/master/secured-by-immudb.svg" width="130px;"/></a>

Amdahl UTS
=========

This is Amdahl's UTS from 1975, a Unix v6 meant for the S/370 architecture. It can only run under VM/370, not directly on the hardware and not on any S/370 emulator. 

This video by Rene' Ferland shows how to install Amdahl UTS and how to operate it. It's quite a fascianting operating system. https://youtu.be/k56qLxG-sUM

Among the programmers working on UNIX v6 and it's twin brother UTS were Eric Schmidt (yes the chairman of Google) and Tom Lyon @aka_pugs on Twitter. 

Contents
========

The <b> 3330</b> DASD and the VM/370 directory entry is really all you need. UTS can *only* run under VM/370. <p>
The source code files are included also as compressed tar files, along with a C compiler and a cross-assembler to build the from .c into S/370 object files. 
 <p>
 A photograph of the original distribution DEC tape is also included.

 <p><p>

Installation
============

Make it visible as a <b> 3330</b> DASD to VM/370 and crate a direcotry entry for UTS like this: (will provide when I find the directory statmeent)

VM/370 Directory Entry 

<pre>
USER UTS AMDAHL 6M 6M G
IPL 220
OPTION ECMODE REALTIMER BMX
CONSOLE 009 3215
SPOOL 00C 2540 READER A
SPOOL 00D 2540 PUNCH A
SPOOL 00E 1403 A
MDISK 150 3330 0 404 UTSSYS WR AMDAHL AMDAHL
MDISK DD0 3330 001 050 UTSSYS WR AMDAHL AMDHAL
MDISK 550 3330 051 050 UTSSYS WR AMDAHL AMDAHL
MDISK 110 3330 101 050 UTSSYS WR AMDAHL AMDAHL
MDISK 220 3330 151 060 UTSSYS WR AMDAHL AMDAHL
MDISK 330 3330 211 160 UTSSYS WR AMDAHL AMDAHL
MDISK 660 3330 371 030 UTSSYS WR AMDAHL AMDAHL
</pre>

This UTS is a verbatim doppel-gaenger of UNIX version 6 for VM/370, if you go and build that system. So this leads me and others to believe this UTS is actually a Unix v6. 

You can find it here: https://www.tuhs.org/Archive/Distributions/IBM/370/


Amdahl UTS is abandonwware and as such no legal entanglements exist for this software. 
<br>
<p><p>
Enjoy

Moshix
<p>
Original upload: Dec 2020
<br><p>
updated: July 21 , 2021<p>
Triest, Italy
