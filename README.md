# Corewar (1337 School Project)
Core War is a 1984 programming game created by D. G. Jones and A. K. Dewdney in which two or more battle programs (called "warriors") compete for control of a virtual computer. These battle programs are written in an abstract assembly language called Redcode.
![Corewar](/images/ex.png)

This project can be broken down into three distinctive parts:
* **The assembler**: this is the program that will compile champions and translate them from the language written them in (assembly language) into “Bytecode”. Bytecode is a machine code, which will be directly interpreted by the virtual
machine.
* **The virtual machine**: It’s the “arena” in which champions will be executed. It offers various functions, all of which will be useful for the battle of the champions.
Obviously, the virtual machine should allow for numerous simultaneous processes.
* **The champion**: It's necessary to create a simple champion just to prove the program functionality.

### How to run:
* git clone https://github.com/rmahjoubi/corewar.git ~/corewar
* cd ~/corewar/
* make
* ./asm [file1.s] [....] (use *zork.s*)
* ./corewar [-v | -d N] [-a] [-n N] <champion1.cor> <...>
  * -v		: Enables visualization
  * -d N	: Dumps memory after N cycles
  * -a		: Prints output from 'aff' (Default is to hide it)

*Pay attention! [-v] has higher priority when used with [-d]*

### Visualization
Visualization is enabled using ncurses library. The native shell (for example, Terminal.app for macos) could show higher permormance than the third-party applications like iTerm. Colors may vary depend on your shell application settings.

### Champions
Check champs file or any other valid file.
