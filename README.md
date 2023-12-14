# Embedded Linux Assignments
## These are my GitHub repos where I’ve stored all my assignment work for the ‘Advanced Embedded Linux Development’ specialization I’m doing on Coursera.

### Here's the Specialization link: 
<a href="https://www.coursera.org/specializations/advanced-embedded-linux-development"> Advanced Embedded Linux Development</a>
## Week-1 Assignments:
### Assignment 1 Repo: 
<a style="text-decoration:none" href="https://github.com/cu-ecen-aeld/assignment-1-ibrahimnazzier" target="_blank">Assignment-1</a>
### Assignment Objectives:
* Getting familiar with assignments environment (setup docker, GitHub actions, and self-hosted runners for automated testing)
* Getting familiar with the Linux command line
* Getting familiar with Shell scripting
* write 2 shell scripts for finding a text in a file and writing text in a specified file.

### Assignment 2 Repo:
<a style="text-decoration:none" href="https://github.com/cu-ecen-aeld/assignment-2-ibrahimnazzier" target="_blank">Assignment-2</a>
* Readings: chapter 2 (File I/O) in Embedded System Programming
### Assignment Objectives:
* Getting familiar with Linux File I/O and its system calls 
* How to open, create, close, write, and read a File I/O
* Replacing old writer script with a c program using I/O syscalls
* Installing a Cross-compiler for ARM processors.
* Writing a Makefile script to compile the .c file for specified ARCH

## Assignment 3 and later assignments Repo:
<a style="text-decoration:none" href="https://github.com/cu-ecen-aeld/assignments-3-and-later-ibrahimnazzier" target="_blank">Assignment-3-and-later Assignmets</a>
### 1. Assignment 3 work
#### Assignment 3 Part one tagged with realize (assignment-3-part-1)
* Readings: chapter 5 (Process Management) in Embedded System Programming
* Work link --> <a style="text-decoration:none" href="https://github.com/cu-ecen-aeld/assignments-3-and-later-ibrahimnazzier/blob/master/examples/systemcalls/systemcalls.c" target="_blank">assignment-3-part-1</a>
* ### Assignment Objectives:
* 3.1.1 What's a process in Linux and its capabilities 
* 3.1.2 Process Creation by Fork() syscall 
* 3.1.3 Process Execution by Exec() syscall family.
* 3.1.4 Process synchronization with wait() syscall
* 3.1.5 How to create a new child Process from an existing process by using (fork(), exec(), and wait()) == system() in user space

#### Assignment 3 Part 2 tagged with the release (assignment-3-part-2)
* Readings: Configuring and Building the Kernel in Mastering Embedded Linux book
* Work link --> <a style="text-decoration:none" href="https://github.com/cu-ecen-aeld/assignments-3-and-later-ibrahimnazzier/blob/master/finder-app/manual-linux.sh" target="_blank">assignment-3-part-2</a>
* ### Assignment Objectives:
 * Configuring and building Linux kernel With native compilation with BusyBox for programming packages on top of the QEMU emulator
  Steps: (All compilation done by an ARM64 cross-compiler)
 * 3.2.1 Install QEMU as our system will run on top of it
 * 3.2.2 Configure and Build the kernel using the Kconfig utility (defconfig used)
 * 3.2.3 Creating base directories
 * 3.2.4 Configure and install BusyBox
 * 3.2.5 Adding libraries dependencies to rootfs/lib64 & /lib
 * 3.2.6 Make device nodes & create initramsfs
## Image for the QEMU after doing these steps:
![Alt text](https://github.com/ibrahimnazzier/Embedded_Linux_Assignments/blob/main/Images/QEMU_Native_Compilation.jpeg)

#### Assignment-4-part-1 tagged with release (assignment-4-part-1)
* Readings: chapter 7 Thread in Linux System Programming book
* Work link --> <a style="text-decoration:none" href="https://github.com/cu-ecen-aeld/assignments-3-and-later-ibrahimnazzier/tree/master/examples/threading" target="_blank">assignment-4-part-1</a>
### Assignment Objectives:
* Understanding concurrency vs Multi-cored threads
* Dealing with Pthread.h API calls
* Using Mutex to lock resources to avoid deadlocks
* Joining threads at the end of a process
* Passing parameters to the thread function

### Assignment-4-part-2 Tagged with the release (assignment-4-complete)
* Readings:
  * Selecting a Build System (Mastering Embedded Linux Programming)
  * Buildroot user manual: <a style="text-decoration:none" href="https://buildroot.org/downloads/manual/manual.html" target="_blank">Buildroot Manual</a>
  * Hello world package example: <a href="https://github.com/cu-ecen-5013/buildroot-external/tree/ecen5013-hello-world">Hello World Example</a>
* Work link --> <a style="text-decoration:none" href="https://github.com/cu-ecen-aeld/assignment-4-ibrahimnazzier" target="_blank">assignment-4-part-2</a>
#### Assignment Objectives:
* Understanding Buildroot build system
* Difference between source tree package & Base_external Package
* Adding External Package using Menuconfig
* Adding Buildroot Repo as a git submodule
* Using another GitHub Repo to build our base_external package
* Using SSH to log in to target (qemu) using loopback address with (dropbear) network package

#### Images for Assignment Configuration and Build:

##### .mk file for the external package to be added to menuconfig:
![Alt text](https://github.com/ibrahimnazzier/Embedded_Linux_Assignments/blob/main/Images/aesd-assignments_mk.png)

##### External package after added to menuconfig:
![Alt text](https://github.com/ibrahimnazzier/Embedded_Linux_Assignments/blob/main/Images/Menuconfig%20for%20external%20package.png)

##### Staging Area for the root file system after Buildroot build:
![Alt text](https://github.com/ibrahimnazzier/Embedded_Linux_Assignments/blob/main/Images/Staging%20area%20for%20the%20root%20dile%20system.png)

##### Running bash scripts and c files added to QEMU by Buildroot External Package:
![Alt text](https://github.com/ibrahimnazzier/Embedded_Linux_Assignments/blob/main/Images/Buildroot%20Qemu.png)
