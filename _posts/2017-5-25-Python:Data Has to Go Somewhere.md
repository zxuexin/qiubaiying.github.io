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
```
   
the length:
`len(bdata) 
 256`

built a new file,write the number:

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

feed:
100
100
56

then close the file:
` fout.close()`


## Structured text files and binary files ##

### text file ###
Text File has follow formats:
1. SCV
2. XML
3. HTML
4. JSON
5. YAML

The usually formats is SCV and HTML.now HTML 5 is supported by most broswers,such as chrome and foxfire.
And it's the tools for XTML5.
1. SCV are ofen used as an exchange format for spreadsheets and databases. we used the standard CSV module liked that:
`import CSV`
 keyword:reader(),writer() and DictReader()
 
2. XML is similary like XTML 5.It's a markup format too,It uses tage to delimit data.
For instance:

```
1  <?xml version="1.0"?>
2  <menu>
3  <dinner hours="3-10">
4     <item price="8.00">spaghetti</item>
5  </dinner>
6  </menu>
```

there are many libraries could used to parse XML.for example: ElementTree

3. HTML(hypertext markup language) is the usually format in web.I read some standard of HTML and CSS in fly.you can search in browers.

4. JSON(JavaScript Object Notation). the main JSON module name *json*.This program can encode(dumps/loads) a JSON string to data or reverse.

5. YAML is similar to JSON,has keys and values, there are third-party library named *yaml* to manipulate it.

### binary file ###
1. HDF5
    It's used mianly in sciece,where fast random access to large datasets in a common requirement.
    Python's interface:h5py(low-level),PyTables(higher-level).
    
## Databases ##
### Relational Databases ###
#### SQL ####
SQL is a declarative language,It has two main categories:1.DDL(data definition language) 2.DML(data manipulation languange)
#### DB-API ####
DB-API is Python's standard API for accessing relational databases.
keyword:connect(),cursor(),execute() and executemany(),fetchone(),fetchmany(),fetchall().
#### SQLite ####
an open source relational database.It's implemented as a standard Python library,and stores databases in normal files.and it's
not full-featured as MySQL and PostgreSQL.But it's also can manages multiple simultaneous users.
#### MySQL ####
There has many book introduced this MySQL,we can buy one to study.
#### PostgreSQL ####
It's a open source relational database too.the Python's most popular driver is psycopg2.If you want build a blog.you can use
flask+PostgreSQL.

#### SQLAIchemy ####
It's a popular cross-database Python library.
### NoSQL Data stores ###
These were written to handle very large data sets, allow more flexible data definitions, or support custom data operations.
#### The dbm Family ####
a format
#### Memcached ####
a cache server
#### Redis ####
a data sturcture server

### Full-Text Databases ###
 Full-Text Databases index almost everything.
