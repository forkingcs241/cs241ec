#CS241   Lawrence Angrave L29 – Homework (4%)
##Thanksgiving homework (aka Exam-review) will be worth 4% of your grade.Bring your printed work to Wed class after break. Some of the questions require research (old slides; wikipedia). 


Netid & Full Name & Section Name (AD0,1,2) at the top of each page!


###Part 1. C (10pts)
1.	What is the difference between a library call and a system call. Give one example of each
2.	What is the * operator in C? What is the & operator? Give an example of each.
3.	How are C strings represented in memory? What is the wrong with malloc(strlen(s)) ?
4.	Why is strncat and strncpy considered safer versions of strcat and strcpy? Write an implementation of strncat and strncpy
5.	On a separate sheet write a program that reads a series of lines from stdin and prints them to sdout using fgets or readline. Your program should stop if a read error or end of file occurs

###Part 2. Memory (10pts)
1.	Briefly explain how a virtual address is converted into a physical address using a multi-level page table. You may use a concrete example e.g. a 64bit machine with 4KB pages
2.	Briefly explain Knuth's memory allocation scheme and the buddy allocation scheme
3.	What is the difference between the MMU and TLB? What is the purpose of each?
4.	Assuming 4KB page tables what is the page number and offset for virtual address 0x12345678  ?
5.	What is the working set? How is it computed?
6.	What is thrashing? When does it occur?
7.	What is a page fault? When is it an error? When is it not an error?

###Part 3. Processes and Threads (10pts)
1.	What resources are shared between threads in the same process?
2.	Explain the actions required to perform a process context switch
3.	Explain the actions required to perform a thread context switch (to a thread in the same process)
4.	How can a process be orphaned? What does the process do about it?
5.	How do you create a process zombie?
6.	Write example code using fork and waitpid to start and wait for another program to finish.

###Part 4. Scheduling (10pts)
1.	Define turnaround time, waiting time and response time in the context of scheduling algorithms.
2.	What is starvation?  Which scheduling policies have the possibility of resulting in starvation?
3.	Which scheduling algorithm results the smallest average wait time?
4.	What scheduling algorithm has the longest average response time?
5.	Why do processes need to be scheduled?
6.	How does bounded wait apply to scheduling? 
7.	Which scheduling algorithm minimizes average initial response time? Waiting time? Total response time?
8.	Describe Round-Robin scheduling and its performance advantages and disadvantages.
9.	Describe the First Come First Serve (FCFS) scheduling algorithm. Explain the performance advantages and disadvantages.
10.	Describe the Pre-emptive and Non-preemptive SJF scheduling algorithms. Explain the performance advantages and disadvantages.
11.	Describe the Preemptive Priority-based scheduling algorithm. Explain the performance advantages and disadvantages.
12.	How does the length of the time quantum affect Round-Robin scheduling?
13.	Define fairness in terms of scheduling algorithms. What are the fairness properties of each of the scheduling disciplines discussed in class?
14.	A process was switched from running to ready state.  Describe the characteristics of the scheduling algorithm being used.

###Part 5. Synchronization and Deadlock(10pts)
1.	Why might a system use a resource allocation graph?
2.	Define circular wait, mutual exclusion, hold and wait, and no preemption. How are these related to deadlock?
3.	What problem does the Banker's Algorithm solve? Provide a worked example to illustrate your main point.
4.	What is the difference between Deadlock Prevention, Deadlock Detection and Deadlock Avoidance? Give examples of each.

###Part 6. IPC and signals(10pts)
1.	What are the differences between a FIFO (named pipe) and a pipe?
2.	How do you redirect standard output to a file?
3.	Write a brief code example that uses dup2 and fork to redirect a child process output to a pipe
4.	What signals can be caught or ignored?
5.	What signals can cannot be caught?
6.	Write brief code that uses sigaction and a signalset to create a SIGALRM handler
7.	Use a brief code example to explain the problem of 'async signal safe'

###Part 7. Networking (10pts)
1.	Explain the purpose of socket, bind, listen accept functions
2.	Write brief (single-threaded) code using getaddrinfo to create a UDP IPv4. Your server should print the contents of the packet or stream to standard out until an exclamation point "!" is read.
3.	Write brief (single-threaded) code using getaddrinfo to create a TCP IPv4 server. Your server should print the contents of the packet or stream to standard out until an exclamation point "!" is read.
4.	Explain the main differences between using select and epoll. Briefly explain what 'edge' and 'level triggered' means in the context of epoll

###Part 8. Networking (10pts)
1.	Describe the services provided by TCP.
5.	How does TCP connection establishment work?
6.	Describe the differences between TCP and UDP.
7.	How does the Domain Name System (DNS) work?
8.	How does DNS use caching?
9.	How is DNS related to IP?
10.	What is NAT?  How does NAT work?

###Part 9 Files (10pts)
1.	Write code that uses read and write to copy the contents of a file
2.	Write brief code to create a symbolic link and hard link to the file /etc/password
3.	Briefly explain permission bits (including sticky and setuid bits) for files and directories
4.	Write brief code to create a function that returns true if a path is a directory.
5.	Write brief code to recursive search user's home directory and sub-directories (use getenv) for a file named "xkcd-functional.png' If the file is found, print the path to standard out

###Part 10. File system (10pts)
1.	Given a description of the block size and i-node structure , what is the maximum size of a file? Assume 10 direct blocks, a pointer to an indirect block, double-indirect, and triple indirect block and a block size of 4KB
2.	In a file system with 4KB files a file uses 10 direct blocks, a completely full indirect block and one double-indirect block which has one entry to a half-full indirect block. How disk blocks does the file use including its content, the inode, and all indirect , double-indirect blocks?
3.	How many i-node reads are required to fetch the file access time at /var/log/dmesg ? Assume the inode of (/) is cached in memory
4.	What information is stored in an i-node?  What information isn’t?
5.	When the size of a block changes in an i-node based file system, how does this change the maximum size of a file?
6.	If an i-node based file system has a certain number of direct and single-indirect blocks, how large is the file?
7.	When would fstat return different information that lstat?

###Part 11. "I know what's in the exam because I wrote it" (bonus 10pt)
On a separate piece of paper (with netid, name,section) design three questions for CS241 final exam: Write one multiple choice question, one short answer and one long answer coding-question . Provide model answers for each of your three questions.
