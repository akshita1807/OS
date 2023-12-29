# Operating System Important Questions✅

# What is an operating system?
An operating system is a program that acts as an intermediary between the user and the
computer hardware. The purpose of an OS is to provide a convenient environment in which user
can execute programs in a convenient and efficient manner.It is a resource allocator responsible
for allocating system resources and a control program which controls the operation of the
computer h/w.

# What is Kernal? (V. Imp)
A kernel is a central component of an operating system. It acts as an interface between the user applications and the hardware. The sole aim of the kernel is to manage the communication between the software (user level applications) and the hardware (CPU, disk memory etc). The main tasks of the kernel are :  
Process management  ,Device management  ,Memory management   ,Interrupt handling  ,I/O communication    

**Types of Kernal?**  
**Monolithic kernel** in an operating system is a kernel that includes all operating system code in a single executable image.eg:  Linux   
**Microkernel** is an OS architecture used for file and memory management, process scheduling, and more. It's similar to a monolithic kernel but allocates space for tasks like file sharing and scheduling. Each service has its address, reducing the kernel and overall OS size.

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

# What is Round Robin Scheduling?  
The Round robin scheduling algorithm is one of the CPU scheduling algorithms in which every process gets a fixed amount of time quantum to execute the process.In this algorithm, every process gets executed cyclically. This means that processes that have their burst time remaining after the expiration of the time quantum are sent back to the ready state and wait for their next turn to complete the execution until it terminates. This processing is done in FIFO order which suggests that processes are executed on a first-come, first-serve basis.

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
If a process has multiple threads of control ,it is called multthreading.
With MultiThreading a single process can perform multiple functions by performing tasks in parallel like one thread can be used to display pictures and other can be used to draw graphics 
MultiThreading enhances resource sharing .

There are basically two types of threads-  
**User level threads**:which works on user level and are visible to the programmer  
**Kernel level threads**: which operates on kernel level
In general user level threads are faster to create and manage than kernal level threads.


There are three different types of thread models -

**Many -to- one**
many user level threads are mapped to a single kernel level thread

**One-to-one**
One single user level thread is mapped to one kernel level thread.

**Many-to-many**
many user level threads are mapped to a smaller or equal number of kernel threads.

# What is Cache ?
Cache memory is a type of high-speed volatile It acts as a buffer between the main memory (RAM) and the central processing unit (CPU). The purpose of cache memory is to store copies of frequently accessed data from main memory to provide quicker access for the CPU, reducing the average time to access memory.computer memory.Cache Memory holds frequently requested data and instructions so that they are immediately available to the CPU when needed.(cache se data delete krne pr wo main memory se delete nhi hota).

# What are Semaphores?
Semaphore is an integer variable,used by vaious process in a mutual exclusive manner to achieve synchronization.

Types  
1.Counting Semaphore (-α to +α)  
2.Binary Semapgore (0 or 1)

# What is a process control block (PCB), and what information does it contain?
A process control block (PCB) is a data structure that holds essential information about a process, including process state, program counter, CPU registers, and memory information.  
🧩Process state-whether the process is in new,ready,running,waiting or terminated state  
🧩Program counter -indicates the address of the next instruction to be executed for the process   
🧩CPU scheduling information- information including priority of the process  
🧩Accounting information -includes the amount of CPU used,time limits etc  
🧩I/O status information -this information includes the list of input output devices allocated to the process  
🧩Memory management information  









# Explain the concept of a Context switch.
Context switching involves saving the context of the running process in PCB so that it can be restored later ,and then loading context or state of another process and run it.

# What are System calls.
System call is a special function that is used by the process to request action from the Operating system.System calls provide the interface between process and operating system so that process can communicate with operating system.

Types of system calls-

🌀 Process Control: handles system calls for process creation, deletion etc.
Example- end,abort,load,wait, execute.

🌀 File Management: file manipulation events like creating, deleting, reading files

🌀Device management: request device,release device, logically attach or detach Device

🌀 Information maintenance:get time,set time,get system data.

🌀 Communication: send, receive messages, transfer information,create communication.

# What is a deadlock in an operating system?
A deadlock in an operating system occurs when two or more processes are blocked and waiting for each other to release resources that they hold, resulting in a situation where none of the processes can proceed.  

**What are the necessary conditions for a deadlock to occur?**  
The necessary conditions for a deadlock to occur are:  

**Mutual exclusion** At least one resource must be held in a non-shareable mode.  
**Hold and wait** A process holding at least one resource is waiting to acquire additional resources held by other processes.  
**No preemption** A resource can only be released voluntarily by the process holding it.  
**Circular wait** A set of processes is waiting for a resource held by another process, which is also waiting for a resource held by another process in the set.  

**How can a deadlock be prevented in an operating system?**  
A deadlock can be prevented in an operating system by employing one or more of the following methods:  

Resource allocation denial- The operating system can refuse resource requests that would lead to a deadlock.  
Resource ordering- The operating system can require processes to request resources in a predetermined order to avoid circular wait.  
Deadlock detection and recovery- The operating system can periodically check for deadlock and take actions to recover from it.  
Preemption- The operating system can preempt resources from one process and allocate them to another process in order to avoid deadlock.  

**How can a deadlock be detected in an operating system?**  
Deadlock can be detected in an operating system by using various algorithms such as the banker's algorithm, the wait-for graph algorithm, or the resource-allocation graph algorithm. These algorithms analyze the system to check for the presence of the necessary conditions for deadlock and determine if a deadlock exists.

**How can a deadlock be resolved in an operating system?**  
A deadlock can be resolved in an operating system by using one or more of the following methods:

**Resource preemption** The operating system can preempt resources from one process and allocate them to another process in order to break the circular wait.  
**Process termination** The operating system can terminate one or more processes involved in the deadlock to release resources and break the deadlock.  
**Rollback** The operating system can roll back the state of one or more processes to a previous checkpoint to release resources and break the deadlock.  
**Timeouts** The operating system can set timeouts for resource requests to prevent processes from waiting indefinitely and avoid deadlock.  

# Bankers Algorithm
The Banker's Algorithm is used to allocate resources to a process considering the availability of the resources and the predetermined maximum need of a process. It checks whether the resources can be allocated to a process or not, for its execution, which is called the “safe state” check.  
It is named the “Banker's Algorithm” because the banks use the same technique to allocate money and sanction loans to their customers or account holders.
(also a solution to deadlock)
# What is a socket? 🔌

-Socket is the end point for communication between processes in client-server architecture.
A socket is identified with an IP address and a port number.

⚠️ Port number must be less than 1024



# What are process scheduling queues?  

A process scheduling is the activity of the removal of running process from the CPU
And selection of another process on the basis of a particular strategy. Operating system manages all PCB in program scheduling queue.  

There are mainly 3 types of scheduling queues:  
 
🍄Job queue-it contains all processes of the system  
🍄Ready queue -the processes which are ready and  has all the resources and is waiting for execution goes to the ready queue   
🍄Device queue- processes waiting for a particular input output device goes to the input queue  



# What is the critical section?🧩

Each process has a segment of code called the critical section in which the process may be changing common variables , updating a table, writing a file and so on.When a process is executing in it's critical section,no other process is allowed to execute in it's critical section i.e no two process are executing in their critical sections at the same time.






# What is fragmentation? Different types of fragmentation?  
Fragmentation occurs in a dynamic memory allocation system when many of the free blocks are too small to satisfy any request.   
**External Fragmentation** External Fragmentation happens when a dynamic memory allocation algorithm allocates some memory and a small piece is left over that cannot be effectively used. If too much external fragmentation occurs, the amount of usable memory is drastically reduced.Total memory space exists to satisfy a request, but it is not contiguous (Unusable space between allocated blocks)  
**Internal Fragmentation** Internal fragmentation is the space wasted inside of allocated memory blocks because of restriction on the allowed sizes of allocated blocks.Allocated memory may be slightly larger than requested memory; this size difference is memory internal to a partition, but
not being used Reduce external fragmentation by compaction (Wasted space within allocated blocks)


# What is aging in the Operating System?
Aging is a technique which helps in avoiding starvation in the resource scheduling system. Starvation occurs when a process is unable to get the resources it needs to run, even though it is waiting for those resources. Aging works by increasing the priority of a process that has been waiting for a long time. This means that the process is more likely to be scheduled to run, even if it has a lower priority than other processes.

# What is Spooling?
Data is transmitted to and held in memory or other volatile storage until the software or computer asks for it to be executed.Spooling is the temporary storage of data for usage and execution by a device, program, or system.

# What is Demand Paging?
Demand paging is a type of swapping done in virtual memory systems. In demand paging, the data is not copied from the disk to the RAM until they are needed or being demanded by some program.The data will not be copied when the data is already available on memeory. This is called lazy evaluation beacuse on;y demanded pages of memory are being swapped from secondary storage to main memory.


**Throughput**  number of processes that complete their execution per time unit  
**Turnaround time** amount of time to execute a particular process  
**Waiting time**  amount of time a process has been waiting in the ready queue   
**Multiprogramming** Runs several programs simultaneously  
**Multitasking** Users can interact with each program while it runs  
**Multiprocessing** Involves multiple processors executing multiple processes  
**short term scheduler** Selects processes from the ready queue and allocates CPU time.  

**medium term scheduler** Swaps processes in and out of memory  
**long term scheduler** Selects processes from job queue and loads them into ready queue.(new se ready state me kis kis process ko leke jana hai wo decide krta hai)  
**Thrashing** Condition when continuous page fault and paging activites occur.Thrashing could lead to a program collapse and degraded CPU performance.
**Race Condition** A race condition is where multiple processes currently read and write to a shared memory locaton and the results depends upon the order of execution
**Burst Time** The time for which cpu executes on a process
**Memory Management Unit** converts logical address to physical address

