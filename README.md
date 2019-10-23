## BTSnoop version 1.0 File Parser
Implementation of a btsnoop file parser in c.

## Usage
./btsnoop_parse.elf btsnoop_hci.log
Sample output:

>>./btsnoop_parse.elf ./btsnoop_sample.log 
btsnoop_header{
	- magic	=> 'b[0x62]  t[0x74]  s[0x73]  n[0x6e]  o[0x6f]  o[0x6f]  p[0x70]  [0x00]  
	- version	=> '0x01'
	- data link type => '0x3ea'
	}
(44)[0x2c] btsnoop_packet_record_t {
	* orignal length => 4
	* included length => 4
	* flags => 2
	* cummulative drops => 0
	* timestamp => Sun 1970-06-21 10:36:15 PDT
	* data
	[0x01] [0x03] [0x0c] [0x00] 

	}
...
 (462)[0x1ce] btsnoop_packet_record_t {
	* orignal length => 71
	* included length => 71
	* flags => 3
	* cummulative drops => 0
	* timestamp => Sun 1970-06-21 10:36:15 PDT
	* data
	[0x04] [0x0e] [0x44] [0x01] [0x02] [0x10] [0x00] [0xff] [0xff] [0xff]
	[0x03] [0xce] [0xff] [0xef] [0xff] [0xff] [0xff] [0xff] [0x7f]
	[0xf2] [0x0f] [0xe8] [0xfe] [0x3f] [0xf7] [0x83] [0xff] [0x1c]
	[0x00] [0x00] [0x00] [0x61] [0xff] [0xff] [0xff] [0x7f] [0xbe]
	[0x20] [0xf5] [0xff] [0xf0] [0xff] [0x07] [0x00] [0x00] [0x00]
	[0x00] [0x00] [0x00] [0x00] [0x00] [0x00] [0x00] [0x00] [0x00]
	[0x00] [0x00] [0x00] [0x00] [0x00] [0x00] [0x00] [0x00] [0x00]
	[0x00] [0x00] [0x00] [0x00] [0x00] [0x00] [0x00] 

	}

## Building
make


