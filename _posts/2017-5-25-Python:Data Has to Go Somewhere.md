# Python:Data's home #
 1. file input/output
 2. Structured Files
 3. Databases
 
## *preface* ##

>   Now, I'm reading the book "Introducing Python:Modern computing in simpule packages".It's neccessary to writed some notes.
    So i builted this blog for write dowm my learning and thinking.because I'm a freashman in programm,if you can figured out 
    the wrong,it's grace and thankful!

## file input/output ##
    keyword:write(),read(),readline(), with,seek()
    
such as:

`fout = open('bfile','wb')
>>> bdata = bytes(range(0,256))
>>> len(bdata)
256
>>> fout = open('bfile','wb')
>>> size = len(bdata)
>>> offset = 0
>>> chunk = 100
>>> while True:
   if offset >size:
     break
   fout.write(bdata[offset:offset+chunk])
   offset += chunk

	
100
100
56
>>> fout.close()`
## Sturctured text files and binary files ##
### text file ###
### binary file ###

## Databases ##
### Relational Databases ###
### NoSQL Data stores ###
### Full-Text Databases ###
