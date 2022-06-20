# File, disk, and system management tools

## System management

| Process management | Memory management | File and disk management | I/O management |
|--|--|--|--|
|OS determines when and how long the CPU will be available to the process.| Each process requires its own separate area of memory -> Memory is allocated to processes when needed and released when no longer needed | Organize information into files and folders | Control access to the input and output devices |
|Schedule execution of processes| OS control the use of memory by addressing blocks of memory and allocate them | Operating systems support many different types file formats | Respond to user keystrokes, mouse clicks |
|||Keep track of the location of every piece of every file on the disk| Interpret I/O requests from user applications |
|||Find each file when required and carry out read and write operations on it.| Arbitrate when >=2 processes require a device at the same time |

- **Process management:** 
    - Process is the program code loaded into a computer's memory and is executed by the CPU.
    - OS maintains a significant amount of information about each process: location of the process in memory, the current state of the process, the address of the last program instruction executed, whether or not the process is awaiting the completion of an I/O operation,...      
    -> Be able to schedule execution of processes
- **Memory management:** Modern operating systems use disk space to create virtual memory. Programs loaded into memory but not currently running    
-> temporarily moved to store on the hard drive    
-> increases the amount of memory available for other programs
- **File and disk management:** When a file too big     
-> Won't be stored in a contiguous location on the disk      
-> Will be written to multiple location     
-> OS have to keep track
- **I/O process:** A I/O request from user process is signaled to the OS using a system call     
-> OS pass the request to the device driver     
-> device driver (program that resides in memory and does nothing until called upon by the OS) relay instructions and data between the OS and a specific hardware device (speaker,...)     
=> OS doesn't need to know the details of hardware -> device-independent + prevents applications from accessing hardware devices directly -> OS arbitrate when aplications compete for resources
# Operating system
- Main functions:
    - Manage the computer system’s resources (The hardware)
    - Provide a user interface
    - Execute programs and services to interact with the user