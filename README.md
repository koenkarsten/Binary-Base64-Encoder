# binary-base64-encoder
Just a small tool to encode 8 bit binary strings with base64, uses no ASCII like a lot of online encoders

## Under the hood
This script takes your 8 bit binary input en does the following
* Chop up the 8 bit blocks to 6 bit blocks
* Convert each 6 bit block to a decimal value
* Lookup the corresponding encoding for each char (in this table)[https://blogs.oracle.com/rammenon/resource/WindowsLiveWriter-WhatisBase64_14272/base64table.jpg]
* Concatenate each of the encoded chars, end return them to the user