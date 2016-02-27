# RC5CoreGen
RC5 Crypto Engine Core Generator in Perl

RC5 is a block cipher invented by Ron Rivest at MIT. It has a variable block size 
(32, 64 or 128 bits), key size (0 to 2040 bits) and number of rounds (0 to 255).  
A key feature of RC5 is the use of data-dependent rotations; one of the goals of 
RC5 was to prompt the study and evaluation of such operations as a cryptographic 
primitive. (Refer to http://en.wikipedia.org/wiki/RC5 for further information.)

This project presents a Perl script that generates VHDL code for RC5 encryption 
and decryption engines. The script asks for desired block size, number of rounds 
and key size, and then generate a complete set of VHDL files (including the test 
benches) that implement the block cipher. The VHDL code is fully synthesizable. 
The architecture of both encryptor and decryptor are pipelined.