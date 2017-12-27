# DRDO_CTF_2017: Stego-1

**Category:** Steganography
**Points:** 50
**Description:**

>An image (hidden.jpg) contains some useful information. You can find it by viewing differently and remembering that everything is in the title.

**Hint:**


## Write-up
The flag in this challenge has been hidden in the image. Its an image steganography challenge. The flag can be found easily using the strings command. The strings command returns each string of printable characters in files.


    $ strings hidden.jpg | grep DRDO
    Flag: DRDO@60_{435VGDIQY}_FLAG!

Therefore, the flag is `DRDO@60_{435VGDIQY}_FLAG!`.