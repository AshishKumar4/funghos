# A simple program #

Developing applications for FunghOS should be very easy. A lot of things are the same as you were used to when creating apps for "normal" OSes. The only things you need to know are functions prototypes, which you can find in the appropriate file in the SVN repository, or you can use this wikipage (SVN is updated more often, though, so it's always better to use SVN).

Now, I will show you a simple program for FunghOS, which will read a string from the keyboard, then print it using various colors.


```
#include <stdio.h>
```

You should be familiar with this first line of code. The most interesting things about it are the functions prototypes, which you can use if you include stdio.h.

```
extern void putch(unsigned char c);

extern void puts(unsigned char *text);

extern void puti(int x);

extern void putx(int x);

extern void txtclr(unsigned char forecolor, unsigned char backcolor);

extern char getchar();

extern char *gets(char *string, int max);

extern int mkwin(int x, int y, int x2, int y2); /* create a window */

extern int rmwin(int winnum); /* delete a window */

```

These functions should be pretty self-explanatory. The only ones I'm going to explain are the mkwin() and rmwin() functions. The mkwin() function will create a window for your program. If you don't create a window at the begining of your app, it will simply run on the terminal from where it was launched. But because sometimes your app could be launched without a terminal window, I prefer creating a window.
So, let's look at our next lines of code...

```
void main()
{
	mkwin(0,0,0,0);
```

Now let's analyze that. If you don't know what's the first line, void main(), you probably won't complete this tutorial because that's a real basic of C. The thing that I'll explain is the mkwin line. As I said before, mkwin creates a window for your program. You just give it 4 arguments : the x,y,x1 and y1 coordinates. If you make all these zeroes, FunghOS will select the coordinates for you dynamically, at each start of the program. It's easier than counting how many "pixels" you want, so let's try it. Now, let's write some text on the display...

```
	puts("Hello FunghOS!\n");
	txtclr(YELLOW,TXTBACKGROUND);
	puts("Hello programmer!\n");
	txtclr(GREEN,TXTBACKGROUND);
	puts("Changing colours is easy, as you see\n");
	txtclr(TXTFOREGROUND,TXTBACKGROUND);
```

The puts() function is a default string-output function. It is nearly the same as printf(), but it can have only one argument and output only strings. If you want to output integers or hexadecimal numbers, use the puti() and putx() functions, respectively. The txtclr() function changes the text foreground and the text background. As you see, it takes these in two arguments, so the function prototype is txtclr(foreground, background). In stdio.h, there are all avaible colors declared, so you can use their names when you want to change the colors. In addition to these, there are also tow other declared colors, TXTFOREGROUND and TXTBACKGROUND. These are used when you want to restore the original colors.

TO BE CONTINUED