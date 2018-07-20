# For what?
This is some tribute to the C-like language compiler which I'll write :)

# Build
First, you need to install Flex and Bison.
For Arch linux/Manjaro
```sudo pacman -Sy flex bison```
after that, copy this repo and cd to it

```
cd ~
git clone https://github.com/lnikon/calculatorUsingFlexAndBison.git calc/
cd calc
```
Then, create the parser
```bison -d calc.y```

after, create the lexer
```flex calc.l```
and after all that, create our *calculator* :)
```gcc calc.tab.c lex.yy.c -o obs```
and run
```./obs```

*THANKS!*

