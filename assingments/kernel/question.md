Here is how I would frame building a basic kernel in Rust as an interview assignment:

"Design and implement a very simple kernel in Rust that does the following:

1. Initializes the core kernel components like memory management, multitasking/scheduling

2. Implements a simple "Hello World" system call that user programs can call to print output

3. Handles timer interrupts - keeps track of uptime/time elapsed

4. Implements functionality to load and execute user programs 

Focus only on the core conceptual parts rather than complex drivers or hardware handling. Modularity and clean interfaces are more important than fancy features.  

Make reasonable assumptions about the target hardware and build environment. You are free to reuse existing crates/libraries for cross-compilation, interfacing with hardware etc. 

Document the key components, control flow, APIs and build instructions in a README.

This assignment allows us to assess the following aspects:

- Understanding of kernel architecture, boot process
- Rust skills - ownership, concurrency, unsafe code
- Design decisions and interfaces 
- Documentation/clarity

You will have 4 days to work on this. We can then spend 60 minutes reviewing it together and discussing potential improvements.

Let me know if you have any other questions!"

The main goals here are to assess OS concepts fundamentals, approach to modular design, and use of Rust without getting too caught up in complex low-level details or advanced features. The review discussion also provides signals about communication ability and learning mindset.