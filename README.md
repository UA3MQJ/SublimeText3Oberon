# Oberon support for Sublime Test 3

## Features

* Syntax support
* Some completions

## Исправлено
- Добавлена подсветка цифр для КП типа 8000L
- Исправлено определение строки и раскраска на имени процедуры
  ```
  PROCEDURE -GetAlignment(VAR a: SHORTINT) "struct {char c; long long l;} _s; *a = (char*)&_s.l - (char*)&_s";
  ```
 кроме - могут быть еще и +, \*, -
 плюс там же камменты и 

- не правильные цвета ARRAY
VAR
  i: SHORTINT; udg: INTEGER; text2ch: ARRAY 2 OF CHAR;

-раскрашивать модули в зеленый - только в IMPORT

## TODO
	
- не правильные цвета, когда тип импортируется: PT3x0A.Melody до точки должно быть зеленым
IMPORT Asm, B := Basic, PT3x0A, B40 := Best40;

VAR
  ace: PT3x0A.Melody; udg: INTEGER;
	
-раскрашивать модули в зеленый
IMPORT b := Basic, d := Debug;
BEGIN
  b.Init; b.CLS;

-раскрашивать в зеленый вызовы определенных функций
