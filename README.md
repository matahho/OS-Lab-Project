# XV6 Operating System Laboratory Project

This project is based on the XV6 open-source operating system developed by MIT. Through various development phases, this project aims to implement system enhancements, custom commands, system calls, scheduling algorithms, synchronization mechanisms, and shared memory capabilities. Each phase introduces new functionalities and modifications to the basic XV6 OS structure, allowing for hands-on learning in OS development.

## Project Phases Overview

### Phase 1: Basic Commands
- **Objective**: Customize boot settings and enhance user interface commands within XV6.
- **Tasks**:
  - Modify XV6 boot configurations.
  - Implement arrow key navigation, including:
    - `ARROW-UP` and `ARROW-DOWN` for command history.
    - Cursor movement between characters.
    - Clear terminal function.
    
- [Phase 1 Description PDF](https://github.com/matahho/OS-Lab-Project/blob/main/Description/Lab1.pdf)
- [Phase 1 Report](https://github.com/matahho/OS-Lab-Project/blob/main/Report/Lab1_report.pdf)
- [Phase 1 Report images](https://github.com/matahho/OS-Lab-Project/blob/main/Report/Lab1_report_images.pdf)

### Phase 2: System Calls
- **Objective**: Create and implement new system calls using register-based argument handling.
- **Tasks**:
  - Implement system calls that retrieve arguments through registers instead of traditional methods.
  - Develop a `copy_file` system call to copy files from a source to a destination.
  - Write additional system calls, such as:
    - `get_uncle_count`: Counts the number of "uncle" processes.
    - `get_process_lifetime`: Calculates the lifespan of a given process.
  
- [Phase 2 Description PDF](https://github.com/matahho/OS-Lab-Project/blob/main/Description/Lab2.pdf)
- [Phase 2 Report](https://github.com/matahho/OS-Lab-Project/blob/main/Report/Lab2_report.pdf)

### Phase 3: Scheduler
- **Objective**: Implement new scheduling features and prevent process starvation.
- **Tasks**:
  - Integrate an Aging feature within XV6 to avoid process starvation.
  - Add multiple scheduling algorithms:
    - **Circular Queue**
    - **LCFS (Last Come First Serve)**
    - **BJF (Best Job First)**
  - Create system calls for scheduling functionalities, such as changing queues for process management.
    
- [Phase 3 Description PDF](https://github.com/matahho/OS-Lab-Project/blob/main/Description/LAB3.pdf)
- [Phase 3 Report](https://github.com/matahho/OS-Lab-Project/blob/main/Report/Lab3_report.pdf)
  
### Phase 4: Synchronization & CPU Coherency
- **Objective**: Enhance process synchronization and measure CPU coherency.
- **Tasks**:
  - Design and implement a `Priority Lock` for process synchronization based on priority, including `acquire` and `release` functions.
  - Introduce new variables in the CPU struct to track system calls per CPU, allowing experimentation with CPU coherency.

- [Phase 4 Description PDF](https://github.com/matahho/OS-Lab-Project/blob/main/Description/LAB4.pdf)
- [Phase 4 Report](https://github.com/matahho/OS-Lab-Project/blob/main/Report/Lab4_report.pdf)

### Phase 5: Shared Memory
- **Objective**: Implement shared memory for inter-process communication.
- **Tasks**:
  - Develop shared memory allocation for XV6 processes.
  - Implement system calls for shared memory management, such as `open` and `close`.

- [Phase 5 Description PDF](https://github.com/matahho/OS-Lab-Project/blob/main/Description/Lab5.pdf)
- [Phase 5 Report](https://github.com/matahho/OS-Lab-Project/blob/main/Report/Lab5_report.pdf)
 
 ## Getting Started

1. **Cloning and Setting Up**: Clone the XV6 project and ensure all dependencies are met.
2. **Build and Run**: Use `make` to build the project and `make qemu` to run in a virtual environment.
3. **Contributions**: Contributions and discussions are welcome; please open issues or pull requests to collaborate.

## References
This project is inspired by MIT's [XV6 OS](https://pdos.csail.mit.edu/6.828/2020/xv6.html). The phases in this project follow educational objectives to enhance understanding in operating systems development.

---

Feel free to explore and contribute to the project as we expand XV6 with these new features!
