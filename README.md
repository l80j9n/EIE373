java c
Department of Electrical and Electronic Engineering 
EIE373 Microcontroller Systems and Interface 
Laboratory Exercise 4: AVR Serial Port Programming
Objective: 
To develop C programs with serial port communication under the Arduino platform.
Introduction: 
This   experiment   introduces   an   application    for   serial   port   communication   inside   the   AVR   microcontroller.
Equipment: 
Atmel   Studio
The Arduino   Starter Kit
Procedure: 
Section A: Write a C program to echo a character 
Write a C program to complete the following   task:
Receive   a   character   from   the   serial port by using the polling   method   and then   send   it   to   a   PC   terminal through the serial port. The baud rate should be 4800.
To view the serial port communication, you should use the freeware   “Tera   Term,”   a PC   terminal. You can locate this software on your computer using the   search   function.

Select “Serial” and an appropriate port for the   serial port   communication. The port   number   should be the same as the port the Arduino connects to your computer.

Select “Setup” from the main   menu and then “Serial port”   .   Set the baud rate to   4800.

Important information: 
Note that you must close Tera Term before you burn your program into Arduino; otherwise, Tera Term holds the serial port, and you cannot burn your program successfully.A character can be sent to the Arduino by   typing it (i.e., using the keyboard). When you type a   character,   Tera Term gets the input   and   sends   it   to   the   Arduino   through   the   serial   port.   When   the Arduino receives   a   character,   it will   send   it to   the   serial port,   and   you   can   read   it   through   Tera Term.
Section B: Write a C program to send and receive strings 
Write a C program to complete the following tasks:
1.       (Do it   once   at the beginning)   Send   “We Are   Ready”   to   the   serial   port代 写EIE373 Microcontroller Systems and Interface Laboratory Exercise 4: AVR Serial Port ProgrammingJava
代做程序编程语言   using   polling.   Note   that the clock frequency of   the Arduino   Start Kit is   16   MHz.
2.       (Do it repeatedly) Receivedata from the serial port   by polling. If   the received string is “Hi”,   your program   should   send   “Bye”   to   the   serial   port.   (Hint:   To   get   a   string   from   the   serial   port, your   program   should   receive   it   character   by   character.   For   example,   if   your   program gets a string “abc”, the characters received from the serial port should be “a” first, and then   “b”, and   finally   “c”.)The string “Hi” can be sent to the Arduino by typing it (i.e., using the keyboard) in Tera Term.   When you type   “Hi”,   Tera   Term   gets   the   input   and   sends   it to   the   Arduino   through   the   serial   port. When the Arduino receives the string, it will send a message “Bye!” to the serial port, and   you can read it through Tera Term (see the   figure   below):
Section C: Write a C program to keep sending and receiving characters 
Write a C program to complete the following tasks using the polling method:
1.       Before you press any keys, the character ‘a’ is printed continuously.
2.       When you press a key (say ‘b’), ten characters of   this key (i.e., ‘b’) are printed out and then   stop.
3.       After that, nothing happens when you press a key other than the first key   (i.e., ‘b’).
4.       When   you   press   the   key   again   (i.e.,   ‘b’),   the   character   ‘a’   is   printed   continuously   (i.e.,   resume).
Set the baud rate of   the PC terminal (i.e., Tera Term) to   9600.
If   your program runs successfully and the setting of   Tera Term   is   correct, you   should   see the   following output:

Section D: Write C programs by using the serial port interrupt 
You should repeat Sections B and C, but this time, you should use the serial port   interrupt   (not   the   polling   method).





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
