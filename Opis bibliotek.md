### Spis treści
* [assert.h](#asserth) - Makro asercji.
* [ctype.h](#ctypeh) - Klasyfikowanie znaków.
* [errno.h](#errnoh) - Deklaracje kodów błędów.
* [float.h](#floath) - Właściwości typów zmiennoprzecinkowych zależne od implementacji.
* [limits.h](#limitsh) - Właściwości typów całkowitych zależne od implementacji.
* [locale.h](#localeh) - Ustawienia międzynarodowe.
* [setjmp.h](#setjmph) - bsługa nielokalnych skoków.
* [signal.h](#signalh) - [Obsługa sygnałów.
* [stdarg.h](#stdargh) - Narzędzia dla funkcji ze zmienną liczbą argumentów.
* [stddef.h](#stddefh) - Standardowe definicje.
* [stdio.h](#stdioh) - Standard Input/Output, czyli standardowe wejście-wyjście.
* [stdlib.h](#stdlibh) - Najbardziej podstawowe funkcje.
* [string.h](#stringh) - Operacje na łańcuchach znaków
* [time.h](#timeh) - Funkcje obsługi czasu.

## assert.h 
#### Makro asercji.

```cpp
assert()
```

## ctype.h
#### Klasyfikowanie znaków.


```cpp
int isalnum(char c);
```
>sprawdza czy znak jest liczbą lub literą 


```cpp
int isalpha(char c); 
```
>sprawdza czy znak jest literą

```cpp
int isblank(char c); 
```
>sprawdza czy znak jest znakiem odstępu służącym do oddzielania wyrazów (standardowymi znakami odstępu są spacja i znak tabulacji) 

```cpp
int iscntrl(char c); 
```
>sprawdza czy znak jest znakiem sterującym 

```cpp
int isdigit(char c); 
```
>sprawdza czy znak jest cyfrą dziesiętna 

```cpp
int isgraph(char c); 
```
>sprawdza czy znak jest znakiem drukowalnym różnym od spacji 

```cpp
int islower(char c); 
```
>sprawdza czy znak jest małą literą 

```cpp
int isprint(char c); 
```
>sprawdza czy znak jest znakiem drukowalnym (włączając w to spację) 

```cpp
int ispuntc(char c);
```
>sprawdza czy znak jest znakiem przestankowym, dla którego ani isspace ani isalnum nie są prawdziwe (standardowo są to wszystkie znaki drukowalne, dla których te funkcje zwracają zero) 

```cpp
int isspace(char c); 
```
>sprawdza czy znak jest tzw. białym znakiem (standardowymi białymi znakami są: spacja, wysunięcie strony '\f', znak przejścia do nowej linii '\n', znak powrotu karetki '\r', tabulacja pozioma '\t' i tabulacja pionowa '\v') 

```cpp
int isupper(char c);
```
>sprawdza czy znak jest dużą literą 

```cpp
int isxdigit(char c); 
```
>sprawdza czy znak jest cyfrą szesnastkową, tj. cyfrą dziesiętną lub literą od 'a' do 'f' niezależnie od wielkości 

```cpp
char tolower(char c);
```
>przekształca go do odpowiedniej małej litery o ile takowa istnieje 

```cpp
char toupper(char c);
```
>przekształca go do odpowiedniej dużej litery o ile takowa istnieje 

## errno.h 
#### Deklaracje kodów błędów.

```cpp
EDOM (makro)
```

```cpp
EILSEQ (makro) [C99]
```

```cpp
ERANGE (makro)
```

```cpp
errno (zmienna)
```

## float.h
#### Właściwości typów zmiennoprzecinkowych zależne od implementacji. 

## limits.h
#### Właściwości typów całkowitych zależne od implementacji. 

## locale.h 
#### Ustawienia międzynarodowe.

```cpp
localeconv()
```

```cpp
setlocale()
```

## math.h
#### Funkcje matematyczne.
```cpp
FP_FAST_FMAF (makro) [C99]
```

```cpp
FP_FAST_FMAL (makro) [C99]
```

```cpp
FP_FAST_FMA (makro) [C99]
```

```cpp
FP_ILOGB0 (makro) [C99]
```

```cpp
FP_ILOGBNAN (makro) [C99]
```

```cpp
FP_INFINITE (makro) [C99]
```

```cpp
FP_NAN (makro) [C99]
```

```cpp
FP_NORMAL (makro) [C99]
```

```cpp
FP_SUBNORMAL (makro) [C99]
```

```cpp
FP_ZERO (makro) [C99]
```

```cpp
HUGE_VALF (makro) [C99]
```

```cpp
HUGE_VALL (makro) [C99]
```

```cpp
HUGE_VAL (makro)
```

```cpp
INFINITY (makro) [C99]
```

```cpp
MATH_ERREXCEPT (makro) [C99]
```

```cpp
MATH_ERRNO (makro) [C99]
```

```cpp
NAN (makro) [C99]
```

```cpp
acosh()
```

```cpp
acos()
```

```cpp
asinh()
```

```cpp
asin()
```

```cpp
atan2()
```

```cpp
atanh()
```

```cpp
atan()
```

```cpp
cbrt() [C99]
```

```cpp
ceil()
```

```cpp
copysign() [C99]
```

```cpp
cosh()
```

```cpp
cos()
```

```cpp
double_t (typ) [C99]
```

```cpp
erfc() [C99]
```

```cpp
erf() [C99]
```

```cpp
exp2() [C99]
```

```cpp
expm1() [C99]
```

```cpp
exp()
```

```cpp
fabs()
```

```cpp
fdim() [C99]
```

```cpp
flaot_t (typ) [C99]
```

```cpp
floor()
```

```cpp
fmax() [C99]
```

```cpp
fma() [C99]
```

```cpp
fmin() [C99]
```

```cpp
fmod()
```

```cpp
fpclassify() [C99]
```

```cpp
frexp()
```

```cpp
hypot() [C99]
```

```cpp
ilogb() [C99]
```

```cpp
isfinite() [C99]
```

```cpp
isgreaterequal() [C99]
```

```cpp
isgreater() [C99]
```

```cpp
isinf() [C99]
```

```cpp
islessequal() [C99]
```

```cpp
islessgreater() [C99]
```

```cpp
isless() [C99]
```

```cpp
isnan() [C99]
```

```cpp
isnormal() [C99]
```

```cpp
isunordered() [C99]
```

```cpp
ldexp()
```

```cpp
lgamma() [C99]
```

```cpp
llrint() [C99]
```

```cpp
llround() [C99]
```

```cpp
log10()
```

```cpp
log1p() [C99]
```

```cpp
log2() [C99]
```

```cpp
logb() [C99]
```

```cpp
log()
```

```cpp
lrint() [C99]
```

```cpp
lround() [C99]
```

```cpp
math_errhandling (makro) [C99]
```

```cpp
modf()
```

```cpp
nan() [C99]
```

```cpp
nearbyint() [C99]
```

```cpp
nextafter() [C99]
```

```cpp
nexttoward() [C99]
```

```cpp
pow()
```

```cpp
remainder() [C99]
```

```cpp
remquo() [C99]
```

```cpp
rint() [C99]
```

```cpp
round() [C99]
```

```cpp
scalbln() [C99]
```

```cpp
scalbn() [C99]
```

```cpp
signbit() [C99]
```

```cpp
sinh()
```

```cpp
sin()
```

```cpp
sqrt()
```

```cpp
tanh()
```

```cpp
tan()
```

```cpp
tgamma() [C99]
```

```cpp
trunc() [C99] 
```

## setjmp.h 
#### Obsługa nielokalnych skoków.

```cpp
longjmp()
```

```cpp
setjmp()
```

## signal.h 
#### Obsługa sygnałów.

```cpp
raise()
```

```cpp
signal()
```

## stdarg.h 
#### Narzędzia dla funkcji ze zmienną liczbą argumentów.

```cpp
va_arg()
```

```cpp
va_end()
```

```cpp
va_start()
```

## stddef.h 
#### Standardowe definicje.

```cpp
offsetof()
```

## stdio.h 
#### Standard Input/Output, czyli standardowe wejście-wyjście. 
```cpp
clearerr()
```

```cpp
fclose()
```

```cpp
feof()
```

```cpp
ferror()
```

```cpp
fflush()
```

```cpp
fgetc()
```

```cpp
fgetpos()
```

```cpp
fgets()
```

```cpp
fopen()
```

```cpp
fprintf()
```

```cpp
fputc()
```

```cpp
fputs()
```

```cpp
fread()
```

```cpp
freopen()
```

```cpp
fscanf()
```

```cpp
fseek()
```

```cpp
fsetpos()
```

```cpp
ftell()
```

```cpp
fwrite()
```

```cpp
getc()
```

```cpp
getchar()
```

```cpp
gets()
```

```cpp
perror()
```

```cpp
printf()
```
> 

```cpp
putc()
```

```cpp
putchar()
```

```cpp
puts()
```

```cpp
remove()
```

```cpp
rename()
```

```cpp
rewind()
```

```cpp
scanf()
```

```cpp
setbuf()
```

```cpp
setvbuf()
```

```cpp
sprintf()
```

```cpp
sscanf()
```

```cpp
tmpfile()
```

```cpp
tmpnam()
```

```cpp
ungetc()
```

```cpp
vfprintf()
```

```cpp
vprintf()
```

```cpp
vsprintf()
```

## stdlib.h 
#### Najbardziej podstawowe funkcje. 

```cpp
abort() 
```

```cpp
abs() 
```

```cpp
atexit() 
```

```cpp
atof() 
```

```cpp
atoi() 
```

```cpp
atol() 
```

```cpp
bsearch() 
```

```cpp
calloc() 
```

```cpp
div() 
```

```cpp
exit() 
```

```cpp
free() 
```

```cpp
getenv() 
```

```cpp
itoa() 
```

```cpp
labs() 
```

```cpp
ldiv() 
```

```cpp
malloc() 
```

```cpp
mblen() 
```

```cpp
mbstowcs() 
```

```cpp
mbtowc() 
```

```cpp
qsort() 
```

```cpp
rand() 
```

```cpp
realloc() 
```

```cpp
srand() 
```

```cpp
strtod() 
```

```cpp
strtol() 
```

```cpp
strtoul() 
```

```cpp
system() 
```

```cpp
wctomb() 
```

```cpp
wcstombs() 
```
## string.h 
#### Operacje na łańcuchach znaków
```cpp
memchr()
```

```cpp
memcmp()
```

```cpp
memcpy()
```

```cpp
memmove()
```

```cpp
memset()
```

```cpp
strcat()
```

```cpp
strchr()
```

```cpp
strcmp()
```

```cpp
strcoll()
```

```cpp
strcpy()
```

```cpp
strcspn()
```

```cpp
strerror()
```

```cpp
strlen()
```

```cpp
strncat()
```

```cpp
strncmp()
```

```cpp
strncpy()
```

```cpp
strpbrk()
```

```cpp
strrchr()
```

```cpp
strspn()
```

```cpp
strstr()
```

```cpp
strtok()
```

```cpp
strxfrm()
```

```cpp
strdup()
```

## time.h 
#### Funkcje obsługi czasu.
```cpp
asctime()
```

```cpp
clock_t clock( void );
```

```cpp
char* ctime(const time_t *wskczasu);
```

```cpp
double difftime(time_t czas1, time_t czas2);
```

```cpp
gmtime()
```

```cpp
struct tm *localtime(const time_t *timep);
```

```cpp
mktime()
```

```cpp
size_t strftime(char *s, size_t max, const char *format, const struct tm *tm);
```

```cpp
time_t time(time_t *wskczasu);
```

```cpp
struct tm {
    int     tm_sec;         /* sekundy od pełnej minuty*/
    int     tm_min;         /* minuty  od pełnej godziny*/
    int     tm_hour;        /* godzina na 24-godzinnym zegarze*/
    int     tm_mday;        /* dzień miesiąca */
    int     tm_mon;         /* miesiąc licząc od zera */
    int     tm_year;        /* rok - 1900 */
    int     tm_wday;        /* dzień tygodnia niedziela ma numer 0*/
    int     tm_yday;        /* dzień roku licząc od zera*/
    int     tm_isdst;       /* znacznik czasu letniego */
};
```
