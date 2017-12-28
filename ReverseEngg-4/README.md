# DRDO_CTF_2017: ReverseEngg-4

**Category:** Reverse Engineering
**Points:** 50
**Description:**

>Challenge is to find the hidden secret information from the linux executable file (reverse_vpn) without executing it. The Clue given is reverse engineering.
**Hint:**


## Write-up
It's a simple challenge. Use the strings command and grep.

>$ strings hidden.jpg | grep DRDO <br/>
>#!GALF_}7B19J68KG{_06@ODRD


Therefore, the flag is `DRDO@60_{GK86J91B7}_FLAG!`.