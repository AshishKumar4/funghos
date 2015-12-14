FunghOS should be secure, fast, light-weight Operating System. It is now in a very early stage, but one day, it will be great :). For other information (in english and czech), you can visit my "main" webpage, houbysoft. The link is here (in the links section, "Houbysoft main page")-->

Credits:
As of now, only me, Jan Dlabal.


---


**Currently working on support for preemptive multitasking**


---

## News ##
31.10.08 **-> added an 'x' button in the right corner of windows for closing the windows**

![http://funghos.googlecode.com/files/FunghOS-v0.04.42-close_buttons.jpg](http://funghos.googlecode.com/files/FunghOS-v0.04.42-close_buttons.jpg)

29.10.08 **-> added new function for removing windows, rmwin, and fixed the ps/2 mouse driver again so that it doesn't overwrite the new character that has been "under" the mouse cursor**

27.10.08 **-> squashed a big bug in malloc, now it should be working without problems, if any, email me ;), and btw, because the bug is squashed, moved the window structures to linked list allocation again, and mouse driver updated.**

25.10.08 **-> commited the new version of the PS/2 mouse driver, now you can select windows by left-clicking into them!**

24.10.08 **-> commited the dvtab, and a BASIC PS/2 MOUSE DRIVER! A screenshot of its output is here :**

![http://funghos.googlecode.com/files/FunghOS-v0.04.42.jpg](http://funghos.googlecode.com/files/FunghOS-v0.04.42.jpg)

23.10.08 **-> added a dvtab - device table to make it easier to make new drivers (I will commit it to SVN soon, along with the PS/2 Mouse driver on which I'm working now)**

**-> added new PC speaker function - beep()**

**-> added new PIT driver function - wait(time in seconds)**

**-> mkwin() now has one parameter less, creating windows is now even simpler ;-)**

**-> windows structures are now dynamically allocated**

**-> released devel version 0.04.1**

**-> added a PC speaker driver**

**-> added a physical pages bitmap, RAM amount detector**

**-> fixed scrolling of windows!**

**-> released version 0.04!**


---

## Current goals ##

-> finish the ps/2 mouse driver


---

## Screenshot ##
**FunghOS v0.04._in Bochs..._**

![http://funghos.googlecode.com/files/FunghOS-v0.04.1.jpg](http://funghos.googlecode.com/files/FunghOS-v0.04.1.jpg) ![http://funghos.googlecode.com/files/FunghOS-v0.04.1-login.jpg](http://funghos.googlecode.com/files/FunghOS-v0.04.1-login.jpg)


---
