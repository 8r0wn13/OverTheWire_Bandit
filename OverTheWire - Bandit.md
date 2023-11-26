# OverTheWire Bandit

## Description
These are exercises spread over 35 levels to get you more familiar with Linux by doing exercises.

## Level 0:
`ssh bandit0@bandit.labs.overthewire.org -p 2220`
Password: `bandit0`
`ll`
`cat readme`

## Level 1:
`ssh bandit1@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 0`
`ll`
`cat ./-`

## Level 2:
`ssh bandit2@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 1`
`ll`
`cat spaces\ in\ this\ filename` or `cat "spaces in this filename"`

## Level 3:
`ssh bandit3@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 2`
`ll`
`cd inhere`
`cat .hidden`

## Level 4:
`ssh bandit4@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 3`
`ll`
`cd inhere`
`cat ./-file00`
`cat ./-file01`
`cat ./-file02`
`cat ./-file03`
`cat ./-file04`
`cat ./-file05`
`cat ./-file06`
`cat ./-file07`

## Level 5:
`ssh bandit5@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 4`
Look for files in the folders which have a size of 1033 bit
`cd maybehere00 && ll`
`cd ../maybehere01 && ll`
`cd ../maybehere02 && ll`
`cd ../maybehere03 && ll`
`cd ../maybehere04 && ll`
`cd ../maybehere05 && ll`
`cd ../maybehere06 && ll`
`cd ../maybehere07 && ll`
`cat .file2`

## Level 6:
`ssh bandit6@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 5`
`find / -user bandit7 -group bandit6 2>&1 | grep -v "Permission denied"`
`cat /var/lib/dpkg/info/bandit7.password`

## Level 7:
`ssh bandit7@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 6`
`find / -name data.txt 2>&1 | grep -v "Permission denied"`
`cat /home/bandit7/data.txt | grep millionth`

## Level 8:
`ssh bandit8@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 7`
`cat data.txt | sort | uniq -u`

## Level 9:
`ssh bandit9@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 8`

## Level 10:
`ssh bandit10@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 9`
`cat data.txt | strings | grep =`

## Level 11:
`ssh bandit11@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 10`
`cat data.txt | base64 -d`

## Level 12:
`ssh bandit12@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 11`
`cat data.txt | tr 'a-zA-Z' 'n-za-mN-ZA-M'`

## Level 13:
`ssh bandit12@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 12`
`mkdir /tmp/blah123`
`cp data.txt /tmp/blah123`
`cd /tmp/blah123`
`cat data.txt` shows that it is a hex dump
`xxd -r data.txt data`
`file data`
`mv data data.gz`
`gzip -d data.gz`
`file data data`
`mv data data2.bz`
`bzip2 -d data2.bz`
`file data2`
`mv data2 data4.gz`
`gzip -d data4.gz`
`file data4`
`mv data4 data4.tar`
`tar -xf data4.tar`
`file data5.bin`
`mv data5.bin data5.tar`
`tar -xf data5.tar`
`file data6.bin`
`mv data6.bin data6.bz`
`bzip2 -d data6.bz`
`file data6`
`mv data6 data6.tar`
`tar -xf data6.tar`
`file data8.bin`
`mv data8.bin data8.gz`
`gzip -d data8.gz`
`file data8`
`cat data8`

## Level 14:
`https://overthewire.org/wargames/bandit/bandit14.html`
`ssh bandit13@bandit.labs.overthewire.org -p 2220`
Password: `password found in level 13`

wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw

















