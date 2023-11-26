Here are the key steps to build a basic kernel in Rust:

1. Set up the build environment:
   - Install Rust toolchain and essential build tools like cargo, gcc etc.
   - Configure a cross-compiler for building to the target architecture. For example, if building for x86_64 systems, you need a cross-compiler to produce x86_64 code.

2. Create a crate for the kernel:
   - Set up the basic crate structure using cargo.
   - The main source file would be `src/main.rs` which will contain the kernel code.
   
3. Initialize kernel components:
   - Set up essential kernel components like memory management, multitasking, interrupts handling. Use Rust abstractions like ownership and borrowing to manage memory correctly.
   - Print basic output to screen to test initial setup.
   
4. Build userspace ABI:
   - Create abstraction layers and APIs for userspace applications to use kernel facilities. For example, system calls, vfs, socket handling etc.
   
5. Implement Drivers:
   - Write architecture specific drivers that can interact with hardware like audio, network, input devices etc.
   
6. Create startup files:
   - Create a linker script, bootloader code and assembly startup files required to set up Rust runtime and kernel state before launching main.rs.
   
7. Build final kernel: 
   - Use cargo to produce final kernel binary in appropriate format to run on real or virtual hardware.
   - Test and debug kernel using emulators like QEMU or actual hardware.
   
8. Iterate and improve:
   - Repeat process by incrementally adding kernel features like networking, filesystem, drivers, security mechanisms etc.

Additionally, there are resources like the Rust OS dev community and projects like the Redox OS that provide information and code samples to help build kernels in Rust.