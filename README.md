# User Thread Context Switching
This assignment implements a user thread library and its round-robin scheduler, say sthread (not
pthread). It exercises how to capture and restore the current execution environment with setjmp( ) and longjmp( ), to
retrieve stack and base pointers from the CPU register set with asm( ), and to copy the current activation record (i.e.,
the stack area of the current function) into a scheduler's memory space upon a context switch to a next thread. We
also use signal( ) and alarm( ) to guarantee a minimum time quantum to run the current thread.


### Files

- sthread.cpp : user thread library and scheduler
- driver.cpp

### Testing
- g++ driver.cpp and run ./a.out
