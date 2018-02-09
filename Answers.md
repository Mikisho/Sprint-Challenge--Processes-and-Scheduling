1. The answer is 
    b. P1: 0 - 64,000;
	   P2: 0 - 64,000 
    * Because, before scheduling process P2, the OS sets the address range regiters to `0 - 64000`.

2. Processes may have 5 states:
    * **New**: also called _*Created*_ is when a process is in the stage of being created. The process under this state awaits for admission to the `ready` state and will be approved or delayed by a longterm. In most cases of desktop computer systems, such admission will be approved automatically. However, the admission might be delayed for a real-time operating systems.

    * **Ready**: this is a state by which ready processes are waiting to have the processor allocated to them. However, at this state CPU will not be working on this process's instructions.

    * **Running**: is a state that the processor starts to execute instructions. This is also the state that a given process is chosen for execution. Thus, a process can run in two modes namely, `Kernel mode or user mode`.

    * **Waiting**: is a state by which a process moves if it needs to wait for a resource. For example a given process might be waiting for a user input, disk access request or a file to become available. 

    * **Terminated or Exit**: this is a state by which a process is moved to once it finishes its execution or terminated by the operating system. In other words, the process has completed.


3. The loop with `write` runs `3000000` times, while `printf` does not. Thus, `write` is an expensive call than copying data into `printf`'s buffer and reducing the number of `write` calls provides a net performace win.


4. `printf` is buffered where as `write` is not. Thus, `printf` does not necessairly calls `write` every time. Moreover, internally, `printf` will use `write` when its buffer is full. 