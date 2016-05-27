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
                       /* 00001111 11111111 11111111 11111111 >> 4 = 00000000 11111111 11111111 11111111 */
                       0x0FFFFFFF >> 4 == 0x00FFFFFF 
                       
Note that the right shift operator is signed. Java, as with many other languages, uses the most significant bit as a 
"sign" bit. A negative number's most significant bit as a "sign" bit. A negative number's most significant bit is
always 1 in Java. A signed shift-right will shift in the value of the sign. So, a binary number that begins with '1'
will shift in 1's. A binary number that shifts that begins with '0' will shift in 0's. Java does bitwise operators
on integers, so be aware!

You can use a third shift operator called the "unsigned shift right" operator: >>> for always shifting in "0" regardless
of the sign. 
