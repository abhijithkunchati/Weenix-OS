Weenix
======
A full operating system, based on Unix, built as a semester long project. 

## Making an OS
I was part of a team that was tasked with developing an OS based on the x86 architecture and should, in theory, compile to an image that can be run on a bare x86 machine. The OS has to be able to run several threads and processes concurrently in kernel mode as well as in user mode, develop the virtual file system (VFS) to be able to provide interface between the kernel and various file systems and a virtual memory (VM) to enable the kernel to manage user address spaces, to run user level code and handle system calls.

## Features
Implemented the following features as part of Weenix: 
* **Procs** - Threads, processes, and synchronization primitives.
* **Drivers** - Device drivers for terminals, disks, and the memory devices `/dev/zero` and `/dev/null`.
* **VFS (Virtual File System)** - A polymorphic interface between the operating system kernel and the various file systems (such as S5FS and device drivers).
* **S5FS (System V File System)** - A file system implementation based on the original Unix file system.
* **VM (Virtual Memory)** - Userspace address space management, running user-level code, servicing system calls, and basically everything else needed to combine all of the previous componenets into a fully functioning operating system. This includes virtual memory maps, handling page faults, memory management via anonymous objects and shadow objects, and system calls (in particular, the `fork` syscall).

## Screenshots
![image](https://github.com/user-attachments/assets/46cb9d60-40d1-40ea-8329-4dbd1c6a287a)
<p align="center">
Running Weenix
</p>

![image](https://github.com/user-attachments/assets/528e8fb6-e827-4a9f-846e-a6338066f44a)
<p align="center">
Fork-and-wait test
</p>

![image](https://github.com/user-attachments/assets/606eea81-07f1-4adf-9b1a-776c3e225d48)
<p align="center">
VFS test
</p>






