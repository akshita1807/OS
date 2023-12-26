# Operating System Important Questions✅

# What is Kernal? (V. Imp)
A kernel is a central component of an operating system. It acts as an interface between the user applications and the hardware. The sole aim of the kernel is to manage the communication between the software (user level applications) and the hardware (CPU, disk memory etc). The main tasks of the kernel are :  
Process management  
Device management  
Memory management   
Interrupt handling  
I/O communication  

**Types of Kernal?**



# What is a process in OS and What are the different states of a process?
A program in execution is called process.  
States of process:  
**New**-Process is in stage of being created.  
**Ready**-It has all the resources it needs to run.  
**Running**-CPU is working on this process's instructions.  
**Waiting**-Process cannot run at the moment,it is waiting for some resource to become available.  
**Terminated**-The process has completed.  

# What is a Scheduling Algorithm? Name different types of scheduling algorithms.
A scheduling algorithm in OS is the algorithm that defines how much CPU time must be allotted to which process and when. There are two types of scheduling algorithms:

**Non-preemptive scheduling algorithms**- For these algorithms, once a process starts running, they are not stopped until completion. That is, under non-preemptive algorithms, processes cannot be pre-empted in favor of other high-priority processes before their runtime is over. 
**Preemptive scheduling algorithms**- These algorithms allow for low-priority processes to be preempted in favor of a high-priority process even if they haven’t run to completion.

# What do you mean by FCFS Algorithm and best advantages of it?
In FCFS Scheduling the process which arrives first in the ready queue is firstly assigned the CPU.In case of a tie, process with smaller process id is executed first.It is always non-preemptive in nature.Jobs are executed on first come, first serve basis.It is a non-preemptive, pre-emptive scheduling algorithm also Easy to understand and implement.  
**Advantages**    
👾 It is simple and easy to understand.   
👾 It can be easily implemented using queue data structure.  
👾 It does not lead to starvation.  
**Disadvantages**    
👾 It does not consider the priority or burst time of the processes.  
👾 It suffers from convoy effect i.e. processes with higher burst time arrived before  
the processes with smaller burst time

# What is virtual memory?
A computer can address more memory than the amount physically installed on the system. This extra memory is actually called virtual memory and it is a section of a hard disk.
**Working**
Computer system has a limited amount of static RAM.When a program gets executed,an instance of the program is loaded into the RAM.This is the process of allocating the memory for the instructions to execute.When the program demands more RAM than available,it will be allocated to the virtual memory.This prevents the program from lacking the necessary RAM to execute.This virtual memory is actually the memory of the hard disk and it is then mapped into the physical memory.
**Advantages**
More processes may be maintained in the main memory  
A process may be larger than all of the main memory  
It allows greater multiprogramming levels by using less of the available (primary) memory for each process.  
It has twice the capacity for addresses as main memory.  
It makes it possible to run more applications at once.  

# What is thread in OS?
Threads are basic unit of execution.They have some of the properties of prcoess that is why they are called lightweight process.Each process can have number of threads executing in it.Each threads contains- A program counter,a register set,a stack.

**Multithreading**

# What is Cache ?
Cache memory is a type of high-speed volatile It acts as a buffer between the main memory (RAM) and the central processing unit (CPU). The purpose of cache memory is to store copies of frequently accessed data from main memory to provide quicker access for the CPU, reducing the average time to access memory.computer memory.Cache Memory holds frequently requested data and instructions so that they are immediately available to the CPU when needed.(cache se data delete krne pr wo main memory se delete nhi hota).

# What is the difference between paging and segmentation?

# What is thrashing in OS?
