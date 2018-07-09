where's this photo taken?
-------------------------

temukan flag dalam foto kucing lucu. 
hint flag: md5 dari nama kota tempat foto kucing lucu diambil

download foto kucing, kemudian extract metadata dari foto menggunakan exiftool.

metadata:

```
vicky@localhost:~$ exiftool kucing_unyu.jpg 
ExifTool Version Number         : 10.60
File Name                       : kucing_unyu.jpg
Directory                       : .
File Size                       : 104 kB
File Modification Date/Time     : 2018:07:08 20:58:05+07:00
File Access Date/Time           : 2018:07:08 20:58:23+07:00
File Inode Change Date/Time     : 2018:07:08 20:58:20+07:00
File Permissions                : rw-rw-r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : None
X Resolution                    : 1
Y Resolution                    : 1
Exif Byte Order                 : Big-endian (Motorola, MM)
Image Description               : Kucing pacil unyu unyu
Make                            : Kamera bukan DSLR
Orientation                     : Horizontal (normal)
Modify Date                     : 1945:08:17 08:00:00
Artist                          : Piccaso
Exif Version                    : 0230
Components Configuration        : Y, Cb, Cr, -
Flashpix Version                : 0100
Owner Name                      : Azka ali
Current IPTC Digest             : af3471d275a87aa7dfc71d9f5dc1defa
City                            : Krung Thep Mahanakhon Amon Ratta
Application Record Version      : 4
Image Width                     : 1108
Image Height                    : 1477
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 1108x1477
Megapixels                      : 1.6
(base) vicky@localhost:~$ 

```
tag lokasi dari foto: 
City: Krung Thep Mahanakhon Amon Ratta

*Krung Thep Mahanakhon Amon Ratta* adalah nama lain dari kota Bangkok,
hasil pencarian dari nama lain bangkok menampilkan nama lain yang lebih panjang
dari nama bangkok yakni Krung Thep Mahanakhon Amon Rattanakosin Mahinthara Yuthaya 
Mahadilok Phop Noppharat Ratchathani Burirom Udomratchaniwet Mahasathan Amon Piman Awatan 
Sathit Sakkathattiya Witsanukam Prasit

```
import hashlib

while True:
   flag = "Krung Thep Mahanakhon Amon Rattanakosin Mahinthara Yuthaya Mahadilok Phop Noppharat Ratchathani Burirom Udomratchaniwet Mahasathan Amon Piman Awatan Sathit Sakkathattiya Witsanukam Prasit"
   print(hashlib.md5(flag.encode('ascii')).hexdigest())
```
flag: CTFX{da02dc63432ef76171359c0f1e2f378b}
