# mini-java-parser
This java parser implements basic functionality of the language, like 
- if-else statements
- switch case
- for-loop
- while loop
- try-catch-throw
- classes

To compile and run the files on Ubuntu, you need to install flex and bison, and then run the following commands
```
yacc -d minijava.y
flex minijava.l
gcc lex.yy.c y.tab.c y.tab.h -o minijava
./minijava < test.txt
```
This is just a parser and not a semantic analyzer.
