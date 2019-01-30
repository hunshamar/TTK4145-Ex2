# Mutex and Channel basics

### What is an atomic operation?
An atomic operation is an operation during which a processor can simultaniously read a location and
write it in the same bus operation, this blocks any other writing or reading of memory until the operation is complete. Atomic implies that the operation is indivisible 

### What is a semaphore?
A semaphore is a variable used to control access to a common resource by multiple processes in a concurrent system such as a multitasking operating system. The semaphore flag signals that the variable is being accessed.

### What is a mutex?
When you have two threads attempting to access a single resource, a mutex variable can be used to signal that one
thread is accessing the resource, thus the other thread has to wait until the mutex is off in order to safely access the resource. A mutex ensured only one thread has access to the resource at any moment.

### What is the difference between a mutex and a binary semaphore?
A semaphore signals wether or not the resource is occupied, a mutex is a locking mechanism for the resource. 

### What is a critical section?
>A critical section is the part of the program that accesses shared resources

### What is the difference between race conditions and data races?
 A race condition is when the system attempts to perform multiple operation simultaniously, 
 data races are when multiple threads in a single processor has conflicting accesses to the memory

### List some advantages of using message passing over lock-based synchronization primitives.
No need for synchronization

### List some advantages of using lock-based synchronization primitives over message passing.
Simpler code
