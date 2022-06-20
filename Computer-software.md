# Operating system
- Main functions:
    - Manage the computer system’s resources (The hardware)
    - Provide a user interface
    - Execute programs and services to interact with the user

# System management
## Process management
- Process is the program code loaded into a computer's memory and is executed by the CPU.
- OS determines when and how long the CPU will be available to the process.
- OS maintains a significant amount of information about each process: location of the process in memory, the current state of the process, the address of the last program instruction executed, whether or not the process is awaiting the completion of an I/O operation,...      
    -> Be able to schedule execution of processes
## Memory management
- Each process requires its own separate area of memory -> Memory is allocated to processes when needed and released when no longer needed
- OS control the use of memory by addressing blocks of memory and allocate them
- Modern operating systems use disk space to create virtual memory. Programs loaded into memory but not currently running    
-> temporarily moved to store on the hard drive    
-> increases the amount of memory available for other programs

## File and disk management
- Organize information into files and folders
- Operating systems support many different types file formats
- When a file too big     
-> Won't be stored in a contiguous location on the disk      
-> Will be written to multiple location     
-> OS have to keep track of the location of every piece of every file on the disk
- Find each file when required and carry out read and write operations on it.
- Typical format of disk management
    - New Technology File System (NTFS): Works well for Windows but  not other OS
    - Hierarchical File System (HFS+): Works well for macOS. Also known as Mac OS Extended or HFS Extended. Can't really be used with other OS's
    - Apple File System (APFS): Used exclusively by macOS running High Sierra or later
    - exFAT: Many good features that feels like a combination of NTFS and FAT32
## I/O management
- Control access to the input and output devices
- Respond to user keystrokes, mouse clicks
- Interpret I/O requests from user applications
- A I/O request from user process is signaled to the OS using a system call     
-> OS pass the request to the device driver     
-> driver relay instructions and data between the OS and a specific hardware device (speaker,...)     
=> OS doesn't need to know the details of hardware -> device-independent + prevents applications from accessing hardware devices directly -> OS arbitrate when >=2 processes require a device at the same time

### Hardware Driver
- Driver: A program that resides in memory and does nothing until called upon by the OS
- Drivers for specific hardware devices:
    - Assembler: Input assembly language program into assembler -> Output an object program + information for the loader to prepare the object program for execution
    - Compiler: Input source program in a "high-level language" -> Output orresponding object program.
    - Loader: A program that places an object program into memory and prepares it for execution



