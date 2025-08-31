# OS Simulator

This project is a simulation of an operating system (OS) written in C. It provides a modular framework for experimenting with and understanding core OS concepts such as memory management, scheduling, system calls, and process management. The project is organized for educational purposes and is suitable for students and enthusiasts learning about operating systems.

## Features

- **Memory Management:** Includes modules for paging, memory allocation, and physical/virtual memory management.
- **CPU Scheduling:** Supports multiple scheduling algorithms, including multi-level queue (MLQ) scheduling.
- **System Calls:** Implements a syscall interface and several example system calls.
- **Process Management:** Simulates process creation, scheduling, and execution.
- **Extensible Design:** Modular source code and header files for easy extension and experimentation.

## Project Structure

```
├── Makefile                # Build instructions
├── include/                # Header files for all modules
├── input/                  # Input files and test cases
│   └── proc/               # Example process scripts
├── obj/                    # Compiled object files (generated)
├── output/                 # Output files from simulation runs
├── src/                    # Source code for all modules
```

### Key Directories and Files
- `src/`: C source files for all OS modules (CPU, memory, scheduler, system calls, etc.)
- `include/`: Header files for each module
- `input/`: Test cases and process scripts for simulation
- `output/`: Output logs/results from running the simulator
- `Makefile`: Build automation for compiling different modules and the full OS

## Building the Project

To build the OS simulator and its modules, use the provided `Makefile`. Open a terminal in the project root and run:

```
make           # Builds the full OS simulator (default target)
make mem       # Builds only the memory management modules
make sched     # Builds only the scheduler module
make clean     # Cleans all build artifacts
```

The resulting binaries (`os`, `mem`, `sched`) will be created in the project root.

## Running the Simulator

After building, you can run the simulator with different input files. Example:

```
./os < input/os_0_mlq_paging
```

Output will be generated in the `output/` directory.

## Customization & Extension

- Add or modify source files in `src/` and headers in `include/` to implement new features or algorithms.
- Add new test cases or process scripts in `input/`.
- Update the `Makefile` as needed for new modules.

## Requirements

- GCC (GNU Compiler Collection)
- pthreads library (for threading support)
- Unix-like environment (Linux, macOS, or WSL recommended)

## License

This project is for educational purposes. Please check with your instructor or course policy before submitting any modifications.

---

**Author:** Kyle Dang

Feel free to contribute or use this project as a learning tool!
