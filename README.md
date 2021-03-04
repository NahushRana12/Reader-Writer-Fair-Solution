Problem Statment
Implement a solution via semaphores and threads to the n reader 1 writer problem.  Fairnessalways matters.  You will accept the number of readers from the command line.  In no case willmore than 16 readers be used and always at least 1 reader will be used.  Each reader must accessa shared counter value 250000000 times in the critical section.  Note, it does not update anything,just “reads”.  For convenience code is below that will do this.  A reader reads just one time and awriter writes just one time.  Each reader needs to print its name when done.  The writer will updatethe value 25000 times and print done.  The writer will also set a shared flag, in-cs, when it entersthe  critical  section  and  reset  it  just  before  it  leaves  the  critical  section.   The  reader  must,  uponentering the critical section, check this flag and write an error message if the flag is set.


How to Compile and run.
1. Open cmd
2. Type gcc -ofname assign4.c -lpthread 
3. a.out 5
