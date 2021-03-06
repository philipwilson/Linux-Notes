## Linux for Systems Programmers
####  Drawing heavily on Stevens and Rago, *Advanced Programming in the UNIX® Environment*, Third Edition, ISBN 978-0-321-63773-4 


### Week 1: Getting Started

* [Overview](Overview/README.md)
    * [Historical Context](Overview/history.md)
    * [Unix Architecture](Overview/arch.md)
    * [Setting up a Linux VM on your computer]()
    * [Logging In](Overview/login.md)
    * [A quick look around](Overview/commandline-intro.md)
        * [Files and Directories](Overview/commandline-intro.md)
        * [shell(bash) introduction](Overview/commandline-intro.md)
        * [man pages](Overview/commandline-intro.md)
    * [ssh/scp introduction](Overview/commandline-intro.md)
    * [git introduction]()
    * [Working with text files](Overview/commandline-intro.md)
    * [Input and Output (file descriptors, stdin/out/err, buffering)](Overview/input-output.md)
    * [Programs and Processes](Overview/programs-processes.md)
    * [Error handling](Overview/error-handling.md)
        * [errno and python programming]()
    * [User Identification](Overview/user-identification.md)
        * [users and groups, superuser and sudo]()
    * [Signals, signal handling](Overview/signals.md)
    * [Time values (epoch calendar, time_t, clock_t)](Overview/time-values.md)
    * [System Calls and Library Functions](Overview/syscalls-library.md)
    * [Summary](Overview/summary.md)


### Week 2: File Operations and Directories

* [Files and File I/O](Files/README.md)
    * [Introduction](Files/introduction.md)
    * [File descriptors](Files/file-descriptors.md)
    * [creat(), open(), read(), write(), lseek(), close()](Files/file-system-calls.md)
    * [atomic operations](Files/file-system-calls.md)
    * [blocks, buffering, and IO efficiency](Files/file-system-calls.md)
    * [file sharing](Files/file-system-calls.md)
    * [dup(), dup2()](Files/file-system-calls.md)
    * [/dev/fd]()
    * [sync(), fsync()](Files/file-system-calls.md)
    * [fcntl()](Files/file-system-calls.md)
    * [ioctl()](Files/file-system-calls.md)
* [Files and Directories]()
    * [stat() and fstat()](Files/file-system-calls.md)
    * [ownership and permissions, setuid](Files/file-system-calls.md)
    * [chown(), chmod(), sticky bit :-)](Files/file-system-calls.md)
    * [size(), truncate()](Files/file-system-calls.md)
    * [link(), unlink(), symbolic links](Files/file-system-calls.md)
    * [file times](Files/file-system-calls.md)
    * [mkdir, rmdir, chdir](Files/file-system-calls.md)
    * [dirent and directory system calls](Files/file-system-calls.md)
    * [special files](Files/file-system-calls.md)
    * [file access permission bits summary](Files/file-system-calls.md)

### Week 3:  File Systems, stdio 

* [Kernel and file system internals]()
    * [Block devices]()
    * [inodes, superblock, blocks]()
    * [Buffer cache]()
    * [Read more](Files/notes.md)
* [Standard I/O Library]()
    * [Streams and FILE objects]()
    * [Stdin, stdout, stderr]()
    * [Opening, reading, writing streams]()
    * [Buffering]()
    * [Line at a time I/O]()
    * [Binary I/O]()
    * [Stdio efficiency]()
    * [Temporary files]()
    * [Implementation details](Files/notes.md)
* [System Data Files]()


### Week 4 & 5:  Memory and Processes


* [Memory management]()
    * [Virtual memory]()
    * [Pageing and swap]()
    * [Hardware support]()
    * [vmstat]()
* [Process Environment]()
    * [main(), exit()]()
    * [Command line args and ENV]()
    * [memory layout, memory allocation]()
    * [shared libraries]()
    * [ELF executable format and loading]()
* [Kernel process table and supporting data structures]()
    * [scheduling]()
    * [/proc interface]()
* [Process Control]()
    * [fork(), wait(), waitpid()]()
    * [exec()]()
    * [race conditions]()
* [Process Relationships]()
* [Control Groups]()

### Week 6  Advanced I/O, Interprocess Communications

* [Signals]()
* [Threads and Thread Control]()
* [Daemon Processes]()
* [Advanced I/O]()
    * [Non-blocking I/O]()
    * [Record-locking]()
    * [I/O multiplexing]()
    * [Asynchronous I/O]()
    * [readv() and writev()]()
    * [Memory-mapped files mmap()]()
* [Interprocess Communications]()
    * [Pipes]()
    * [Coprocesses]()
    * [FIFOs]()
    * [Shared Memory]()
    * [Semaphores]()

### Week 7 and 8  Network Programming

* [Network Programming and Sockets]()
* [Terminal IO]()

* [Systems Programming Examples]()
    * [Simple Shell]()
    * [Simple HTTP Server]()
    * [Containers from scratch]()


* [Kernel Bootstrap Mechanics]()
* [Syscall Implementation]()

* [Useful links](LINKS.md)
* [Contributors](contributors.md)
