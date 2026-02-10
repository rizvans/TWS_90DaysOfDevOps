# Core components of Linux - 
There are basically three components in Linux. ASK...which stands for Application, Shell and Kernel.
Application - Notepad, vim etc
Shell - we write commands here
Kernel - Program written in Program C to communicate with Hardware
Hardware - RAM, MOnitor, Hard Disk


Kernel is a program which is written in C Language.
We will write shell commands in shell. Shell will communicate with Kernel and transalte for kernel in a understandable langugage. Then kernel will communicate with Hardware and perform the operations.

# How processes are created and managed?
Processes in Linux are created using a fork() system call to duplicate an existing process, followed typically by an exec() system call to load a new program. They are managed by the kernel, which assigns a unique Process ID (PID) to each, handles scheduling, and responds to signals for control and termination.

# What systemd does and why it matters?
1. Systemd is the default manager of the linux system.
2. It starts the system.
3. Runs required services like network, docker,SSH.
4. Keep checking if services are running properly.
5. Stops services safely when system shuts down.

systemd matters because it starts many services at a time. We can start, stop or restart services by using sytemctl. If any service crash then systemd restart it automatically.systemd keeps logs so you can find issues quickly
