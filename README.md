# Oberon support for Sublime Test 3

## Features

* Syntax support
* Some completions

## Исправлено
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
