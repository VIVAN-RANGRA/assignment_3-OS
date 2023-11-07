# assignment_3-OS

A simple Memory Management System (MeMS) implementation using the mmap and munmap system calls for memory allocation and deallocation. The system manages memory chunks efficiently by organizing them in a chain of nodes.

Functions

Initialization and Cleanup:
mems_init(): Initializes the MeMS system by setting up the initial variables.
mems_finish(): Cleans up the MeMS system by unmapping all allocated memory and resetting global variables.

Memory Management Functions:
mems_malloc(size_t size): Allocates memory using the MeMS system.
mems_free(void *v_ptr): Frees memory pointed by a virtual address.
mems_get(void *v_ptr): Retrieves the physical address associated with a given virtual address within the MeMS system.

Statistics and Printing:
mems_print_stats(): Prints statistics about the MeMS system, including utilized and unused memory, main and sub-chain node details, pages used, and sub-chain length array information.

Helper Functions:
split_subChainNode: Divides a sub-chain node into smaller chunks to efficiently allocate memory.

The MeMS system manages memory segments efficiently, handling allocation and deallocation using a free list. It's designed to be integrated into a larger application for effective memory management. To use this system, integrate it into a program containing the main() function and necessary library dependencies, then compile and execute it.
