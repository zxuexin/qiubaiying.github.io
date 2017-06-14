### **Preface** ###
  nowday,I'm read the book K&R,the whole name  is the C program language.It's really a gelegant,wounderful book.Otherwise i
had learning C language before,but this book alse can tell you how to code C in a great way.so i decide to read it and write 
some notes.

##### Charpeter 4-Functions and Program Structure ####
*  4.1 Basics of Functions

Each function definiton has the form
```
return-type function-name(argument declarations)
    {
         declarations and statements
     }
```     
  The return-type and conversation argument can omitted.If need return a value from called function to its caller.Shall use bellow expression:
  
    return expression;
    
* 4.2 Functions Returning Non-integers
  Don't write the type will not have return type.It can also declarate the function with *double* *float* *char* etc.
  also we can use *expression* to converted to the type of function.
  
* 4.3 External Variables
  External variables and functions are globally accessible,they existence pernament,and convenient to change values
  
* 4.4 Scope Rules
  External variables should be declaration in the in definition file like `int x=1;`
  and only declarate in the other file like `int x;`,needn't write the value,and the declaration must lie ahead of file that suffice the whole file.
  
* 4.5 Header Files
To seprate the function to splited file,and tradeoff which one put which.
the examine in the book is calculate.seprate the `main.c` and head file `calc.h` to share the declaration and definition,and other file for function and storage.
seperate the file is necessary for much larger program to organization and managerment.

* 4.6 Static Variable

  

