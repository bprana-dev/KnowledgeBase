## Black hole of linux				
/dev/null
	- special file
	- char device files
	- null device
	- major:1 minor:3
	- owned by root
	- discards anything written to it	--> data simply disappears
	- return EOF when read from it 

## Use cases
	- eliminate standrad debug prints
	- eliminate error prints
	- empty a file/ clear file contents	
	
## How I use this at work
	- I use it to suppress the output during shell script execution consisting of debug prints during testing.
