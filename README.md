# CRC16
Program that calculates the CRC-16 value for a given file and which can also verify the correctness of a given file that already has a CRC-16 value appended to it,

**Author: [Ganesh Pandey](http://ganeshpandey.com.np/)**
## Usage

#### Used CRC polynomial:
x^16+x^10+x^8+x^7+x^3+1
## Program operation:
  1. The program compile from the command line.
  2. Take two (2) command line parameters.
  3. The first command line parameter will be a flag value that identifies the mode of operation: “c”
      for calculating a CRC value, or “v” for verifying a CRC value.
  4. The second command line parameter will be the name of the file to be examined. The file should
     be a text file that is in the same folder as the program executable.

### clone Repo

    $ git clone https://github.com/GPandey515/CRC16.git
### compile and Run

    $ javac Crcheck.java
    
    $ java Crcheck c file.txt // checksum calculate
![alt tag](https://raw.githubusercontent.com/GPandey515/CRC16/master/c.png)

    $ java Crcheck v file.crc // checksum verification
![alt tag](https://raw.githubusercontent.com/GPandey515/CRC16/master/v.png)
    
# Warning:
Valid input files will be ASCII files that contain printable data.The raw input file will consist of ASCII data of varying length up to 512 bytes, with the last 8 bytes
reserved for the checksum. (Note: The CRC or checksum will be a 16 bit integer, or 4 hexadecimal digits,
which will fill the last 4 bytes/characters, the leading 4 characters should be zeroes.)

##### Note: This program is provided 'AS IS', without warranty of any kind, so use it at your own risk.

