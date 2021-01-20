# UTS
This is Amdahl's UTS from 1975, a Unix v6 meant for the S/370 architecture. It can only run under VM/370, not directly on the hardware. 

Installation

Make it visible as a 2314 to VM/370 and crate a direcotry entry for UTS like this: (will provide when I find the directory statmeent)

VM/370 Directory Entry (thanks to jy99)
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

This UTS is a verbatim doppel-gaenger of UNIX version 6 for VM/370, if you go and build lthat system. So this leads me and others to believe this UTS is actually a Unix v6. 

You can find it here: https://www.tuhs.org/Archive/Distributions/IBM/370/




Enjoy

Moshix

Dec 2020
