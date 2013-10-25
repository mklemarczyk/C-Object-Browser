assert.h 

Makro asercji.
* assert() 

ctype.h 

Klasyfikowanie znaków. 

· isalnum() - sprawdza czy znak jest liczbą lub literą 

o int isalnum(char c); 

· isalpha() - sprawdza czy znak jest literą 

o int isalpha(char c); 

· isblank() [C99] - sprawdza czy znak jest znakiem odstępu służącym do oddzielania wyrazów (standardowymi znakami odstępu są spacja i znak tabulacji) 

o int isblank(char c); 

· iscntrl()sprawdza czy znak jest znakiem sterującym 

o int iscntrl(char c); 

· isdigit()sprawdza czy znak jest cyfrą dziesiętna 

o int isdigit(char c); 

· isgraph()sprawdza czy znak jest znakiem drukowalnym różnym od spacji 

o int isgraph(char c); 

· islower()sprawdza czy znak jest małą literą 

o int islower(char c); 

· isprint()sprawdza czy znak jest znakiem drukowalnym (włączając w to spację) 

o int isprint(char c); 

· ispunct()sprawdza czy znak jest znakiem przestankowym, dla którego ani isspace ani isalnum nie są prawdziwe (standardowo są to wszystkie znaki drukowalne, dla których te funkcje zwracają zero) 

o int ispuntc(char c); 

· isspace()sprawdza czy znak jest tzw. białym znakiem (standardowymi białymi znakami są: spacja, wysunięcie strony '\f', znak przejścia do nowej linii '\n', znak powrotu karetki '\r', tabulacja pozioma '\t' i tabulacja pionowa '\v') 

o int isspace(char c); 

· isupper()sprawdza czy znak jest dużą literą 

o int isupper(char c); 

· isxdigit()sprawdza czy znak jest cyfrą szesnastkową, tj. cyfrą dziesiętną lub literą od 'a' do 'f' niezależnie od wielkości 

o int isxdigit(char c); 

· tolower()przekształca go do odpowiedniej małej litery o ile takowa istnieje 

o char tolower(char c); 

· toupper()przekształca go do odpowiedniej dużej litery o ile takowa istnieje 

o char toupper(char c); 

errno.h 

Deklaracje kodów błędów. * EDOM (makro) * EILSEQ (makro) [C99] * ERANGE (makro) * errno (zmienna) 

float.h 

Właściwości typów zmiennoprzecinkowych zależne od implementacji. 

limits.h 

Właściwości typów całkowitych zależne od implementacji. 

locale.h 

Ustawienia międzynarodowe. * localeconv() * setlocale() 

math.h 

Funkcje matematyczne. * FP_FAST_FMAF (makro) [C99] * FP_FAST_FMAL (makro) [C99] * FP_FAST_FMA (makro) [C99] * FP_ILOGB0 (makro) [C99] * FP_ILOGBNAN (makro) [C99] * FP_INFINITE (makro) [C99] * FP_NAN (makro) [C99] * FP_NORMAL (makro) [C99] * FP_SUBNORMAL (makro) [C99] * FP_ZERO (makro) [C99] * HUGE_VALF (makro) [C99] * HUGE_VALL (makro) [C99] * HUGE_VAL (makro) * INFINITY (makro) [C99] * MATH_ERREXCEPT (makro) [C99] * MATH_ERRNO (makro) [C99] * NAN (makro) [C99] * acosh() * acos() * asinh() * asin() * atan2() * atanh() * atan() * cbrt() [C99] * ceil() * copysign() [C99] * cosh() * cos() * double_t (typ) [C99] * erfc() [C99] * erf() [C99] * exp2() [C99] * expm1() [C99] * exp() * fabs() * fdim() [C99] * flaot_t (typ) [C99] * floor() * fmax() [C99] * fma() [C99] * fmin() [C99] * fmod() * fpclassify() [C99] * frexp() * hypot() [C99] * ilogb() [C99] * isfinite() [C99] * isgreaterequal() [C99] * isgreater() [C99] * isinf() [C99] * islessequal() [C99] * islessgreater() [C99] * isless() [C99] * isnan() [C99] * isnormal() [C99] * isunordered() [C99] * ldexp() * lgamma() [C99] * llrint() [C99] * llround() [C99] * log10() * log1p() [C99] * log2() [C99] * logb() [C99] * log() * lrint() [C99] * lround() [C99] * math_errhandling (makro) [C99] * modf() * nan() [C99] * nearbyint() [C99] * nextafter() [C99] * nexttoward() [C99] * pow() * remainder() [C99] * remquo() [C99] * rint() [C99] * round() [C99] * scalbln() [C99] * scalbn() [C99] * signbit() [C99] * sinh() * sin() * sqrt() * tanh() * tan() * tgamma() [C99] * trunc() [C99] 

setjmp.h 

Obsługa nielokalnych skoków. * longjmp() * setjmp() 

signal.h 

Obsługa sygnałów. * raise() * signal() 

stdarg.h 

Narzędzia dla funkcji ze zmienną liczbą argumentów. * va_arg() * va_end() * va_start() 

stddef.h 

Standardowe definicje. * offsetof() 

stdio.h 

Standard Input/Output, czyli standardowe wejście-wyjście. * clearerr() * fclose() * feof() * ferror() * fflush() * fgetc() * fgetpos() * fgets() * fopen() * fprintf() * fputc() * fputs() * fread() * freopen() * fscanf() * fseek() * fsetpos() * ftell() * fwrite() * getc() * getchar() * gets() * perror() * printf() * putc() * putchar() * puts() * remove() * rename() * rewind() * scanf() * setbuf() * setvbuf() * sprintf() * sscanf() * tmpfile() * tmpnam() * ungetc() * vfprintf() * vprintf() * vsprintf() 

stdlib.h 

Najbardziej podstawowe funkcje. * abort() * abs() * atexit() * atof() * atoi() * atol() * bsearch() * calloc() * div() * exit() * free() * getenv() * itoa() * labs() * ldiv() * malloc() * mblen() * mbstowcs() * mbtowc() * qsort() * rand() * realloc() * srand() * strtod() * strtol() * strtoul() * system() * wctomb() * wcstombs() 

string.h 

Operacje na łańcuchach znaków * memchr() * memcmp() * memcpy() * memmove() * memset() * strcat() * strchr() * strcmp() * strcoll() * strcpy() * strcspn() * strerror() * strlen() * strncat() * strncmp() * strncpy() * strpbrk() * strrchr() * strspn() * strstr() * strtok() * strxfrm() * strdup() 

time.h 

Funkcje obsługi czasu. * asctime() * clock() * ctime() * difftime() * gmtime() * localtime() * mktime() * strftime() * time() 

· tm (struktura) 
