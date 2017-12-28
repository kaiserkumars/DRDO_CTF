# DRDO_CTF_2017: Stego-1

**Category:** Steganography
**Points:** 50
**Description:**

>An image (hidden.jpg) contains some useful information. You can find it by viewing differently and remembering that everything is in the title.

**Hint:**


## Write-up
The flag in this challenge has been hidden in the image. Its an image steganography challenge. The flag can be found easily using the strings command. The strings command returns each string of printable characters in files.


    $ strings hidden.jpg | grep DRDO
   				DRDO@60_{435VGDIQY}_FLAG!
                <rdf:Description xmlns:dc="http://purl.org/dc/elements/1.1/"/><rdf:Description xmlns:dc="http://purl.org/dc/elements/1.1/"><dc:title><rdf:Alt xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"><rdf:li xml:lang="x-default">DRDO@60_{435VGDIQY}_FLAG!</rdf:li></rdf:Alt>
                        </dc:title><dc:description><rdf:Alt xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"><rdf:li xml:lang="x-default">DRDO@60_{435VGDIQY}_FLAG!</rdf:li></rdf:Alt>

Therefore, the flag is `DRDO@60_{435VGDIQY}_FLAG!`.