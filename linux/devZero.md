## Infinite source of zeros
/dev/zero
	- special file
	- char device files
	- zero device
	- major:1 minor:5
	- discards anything written to it
	- return endless streams of zeros when read from it 
	- creates file filled with zeros
	- owned by root

## Use cases
		- format a disk
		- create dummy files for experiments
		- create temporary swap files
		- zero filled memory
			- can be used with mmap

## How I use this at work
	- I used it to create a ddi file for linux image creation
		- example dd if=/dev/zero of=test.ddi bs=1 seek=2GB
			- this will create the test.ddi file stuffed with zero
			- checked size du -h  it will be zero

