**STATUS** : This is a description of building the old versions of DragonOS (0.06 and below). It's provided here for completeness.

# Introduction #
The kernel (kernel.bin) is the main component of the OS. It is responsible for setting up and handling the GDTs, IDTs, ISRs, IRQs, memory management routines, and so on. There are several scripts which automate the task of building the kernel (and the OS).


# kernel-i386 (alpha-0.1-1) Details #
In this release there are several scripts in the root directory of the distribution. You will require the use of a unix based OS (such as Linux), the GNU compiler collection (gcc and ld specifically), nasm 2.x, and QEMU to be able to build the kernel.

**build.sh** allows you to build kernel.bin (which would then be located in the ./bin directory.) It compiles all the .c and .asm files in the src directory (files must be added manually)

**updimg.sh** allows you to place kernel.bin onto a floppy disk image (floppy.img)

**runqemu.sh** uses QEMU to test floppy.img.