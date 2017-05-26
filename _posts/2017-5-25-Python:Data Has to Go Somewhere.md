# Python:Data's home #
 1. file input/output
 2. Structured Files
 3. Databases
 
## *preface* ##

>       Now, I'm reading the book "Introducing Python:Modern computing in simpule packages".It's neccessary to write some notes.
    So i built this blog for write dowm my learning and thinking.because I'm a freashman in program,if you can figured out 
    the wrong,it's graceful and thankful!

## file input/output ##
> keyword:write(),open(),read(),readline(), with,seek()
    
such as:

```
fout = open('bfile','wb')
bdata = bytes(range(0,256))
len(bdata)
``` 
answer:
256

```
fout = open('bfile','wb')
size = len(bdata)
offset = 0
chunk = 100
while True:
    if offset >size:
        break
    fout.write(bdata[offset:offset+chunk])
    offset += chunk
```
answer:
100
100
56

then close the file:
` fout.close()`


## Sturctured text files and binary files ##
Text File has follow formats:
1. SCV
2. XML
3. HTML
4. JSON
5. YAML

The usually formats is SCV and HTML.now HTML 5 is supported by most broswers,such as chrome and foxfire.
And it's the tools for XTML5.

### text file ###
### binary file ###

## Databases ##
### Relational Databases ###
### NoSQL Data stores ###
### Full-Text Databases ###
