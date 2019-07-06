C 101 https://overiq.com/c-programming-101/keywords-and-identifiers/#keywords

C operators https://www.programiz.com/c-programming/c-operators

vim basics https://www.radford.edu/~mhtay/CPSC120/VIM_Editor_Commands.htm

Need to know:

gcc   > to compile files

KEYWORDS:

AUTO

BREAK

CHAR

CONST

CONTINUE

DEFAULT

DO

DOUBLE

ELSE

ENUM

EXTERN

FLOAT

IF

INT

LONG

REGISTER

RETURN

SHORT

SIGNED

SIZEOF

STATIC

STRUCT

TYPEDEF

UNION

UNSIGNED

VOID

VALATILE

WHILE


CASE !FORBIDDEN!
FOR !FORBIDDEN!
GOTO !FORBIDDEN!
SWITCH !FORBIDDEN!
DO...WHILE !FORBIDDEN!


ex05: 

#include <unistd.h>

void  ft_putchar(char all)
{
  write(1, &all, 1);
}

void  ft_print_comb(void)
{
  char a;
  char b;
  char c;
  
  a = '0' - 1;
  while (a++ <= 7)
  {
    ft_putchar('a');
    b = '0';
    while (b++ <= 8)
    {
      ft_putchar(b);
      c = '1';
      while (c++ <= 9)
      {
        ft_putchar(c);
        ft_putchar(',');
        ft_putchar(' ');
      }
    }
  }
}

int   main(void)
{
  ft_print_comb();
  return (0);
}

