A GZip project has a lot of bit manipulation. 

#Shift Happens
Some of the most basic operations on bits is shifting in the form of shift left and shift right. In Java, operators
are << and >>. Here is what they do:

                       /*  00000001 << 1 = 00000010 */
                       1 << 1 == 2
                       /*  00000001 << 3 = 0000100 */
                       1 << 3 == 8
                       /* 11111111 11111111 11111111 11110000 >> 4 = 11111111 11111111 11111111 11111111*/
                       0xFFFFFFF0 >>4 == 0xFFFFFFFF
