# Mutex and Channel basics

### What is an atomic operation?
> An atomic operation is an operation which must complete before anything else is done.

### What is a semaphore?
> A semaphore is a kind of flag which is used to signal whether a function or set of code is available or already in use. Binary - 1 or 0, counting - increments when joined, and decrements when left.
- Can be initialized to any value but, in "runtime" it can only be incremented or decremented. 
- If a thread decrement a semaphore and the result is negative, the thread blocks itself and will only continue until another tread increments the semaphore.  

### What is a mutex?
> A mutex, mutual exclusion, is a program object which blocks access to an amount of code if another thread has already activated the mutex and not yet unlocked it.

### What is the difference between a mutex and a binary semaphore?
> A mutex is a locking mechanism, while a binary semaphore is a signaling mechanism.

### What is a critical section?
> A critical section is the part of a program which accesses shared resources.

### What is the difference between race conditions and data races?
 > *Your answer here*
 - Data race
 When two or more operations that are not synchronized tries to access the same memory location and at least one is write.
 - Race conditions
 Flaws in the timing or ordering of events that can lead to erroneous programing bevahior. 

### List some advantages of using message passing over lock-based synchronization primitives.
> No data races or deadlocks -> easier to avoid bugs.
> Can pass data between threads and processes.
> More scalable.

### List some advantages of using lock-based synchronization primitives over message passing.
> Easier algorithms
> Works in most languages
> 
