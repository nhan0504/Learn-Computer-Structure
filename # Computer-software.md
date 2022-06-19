# File, disk, and system management tools
## File management

## Disk management

## System management
- Main functions:
    - Process management: 
        - The process is the program code is loaded into a computer's memory and is executed by the CPU. 
        - OS determines when and how long the CPU will be available to the process. 
        - OS maintains a significant amount of information about each process: location of the process in memory, the current state of the process, the address of the last program instruction executed, whether or not the process is awaiting the completion of an I/O operation,... -> Be able to schedule execution of processes
    - Memory management:
        - Each process requires its own separate area of memory -> Memory is allocated to processes when needed and released when no longer needed 
        - OS control the use of memory by addressing blocks of memory and allocate them
        - Modern operating systems use disk space to create virtual memory. Programs loaded into memory but not currently running -> temporarily moved to store on the hard drive -> increases the amount of memory available for other programs
    - File and disk management
        - File management: 
            - Organize information into files and folders
            - Operating systems support many different types file formats
        - Disk management:
            - New Technology File System (NTFS): Works well for Windows but not other operating systems
            - Hierarchical File System (HFS+): Works well for macOS. Also known as Mac OS Extended or HFS Extended. Cannot really be used with other OS’s
            - Apple File System (APFS): Used exclusively by macOS running High Sierra or later
            - exFAT - many good features that feels like a combination of NTFS and FAT32
            - I/O system management
# Operating system
- Main functions:
    - Manage the computer system’s resources (The hardware)
    - Provide a user interface
    - Execute programs and services to interact with the user