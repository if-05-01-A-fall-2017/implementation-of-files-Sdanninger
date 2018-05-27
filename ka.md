1.)
  a.)
  250GB => 262 144 000
  262 144 000 Block

  b.)
  262 144 000

  c.)
  29bit (next id)

  d.)
  262 144 000 / 29 = 9 039 448 B for table
  + additionally for directory table

2.)
  a.)
  107834590 - 10 = 107834590 // skip 0 to 9
  107834590 - 256 = 107834334 // single indirect
  107834334 -65536  = 107768798 //double indirect
  107768798 - 16777216 = 91057118 //triple indirect
  91057118 - 4294967296 = - // so read this block


  b.)
  107834590
  calculate which block contains the position

  107834590 / 1024 = 105307te

  read the fat from start 107835 until you reach your Block

  skip the 107834590 % 1024 bytes

  3.)
    Assuming that there are at most an triple indirect block

    1KB
    10 * 1 KB = 10KB// first 10 data blocks
    1024KB/4B * 1024KB = 262,144 MB
    (1024/4B)**2 * 1024KB = 67,108864 GB
    (1024/4B)**2 * 1024KB = 17,179869184 TB
    around 17.5 TB

    4KB
    4096KB/4B * 4096KB = 4.194304 GB
    (4096/4B)**2 * 4096KB = 4. 294 967 296 TB
    (4096/4B)**2 * 4096KB = 4. 398 046 511 104 EB

  4.)

    Assuming that there at most an triple indirect block

    512B
    MAX SIZE around 1. 073 741 824 GB

    1024 B
    MAX SIZE around 17. 179 869 184 GB
