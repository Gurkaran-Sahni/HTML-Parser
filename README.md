# HTML-Parser

Please note that if you are using flex, you need to add the line "%option nounput yylineno" to the first section of your lex input file to get the yylineno to print correctly.  
(without the quotes!)name : value. name describes the the piece of info. 
<open html tag>value is the actual thing. 
<html>config.in is the input file.

Q)How to define a simple lex input file that will recognize tokens like above.
Ans)
->myscanner.l
->myscanner.h defines symbol <open_tag_encountered> for each type of token.
->Actually,they are the tokens which the scanner has to recognise.
->Basically lex.yy.c is scanner.
->We write a C program that utilizes the lex.yy.c program
