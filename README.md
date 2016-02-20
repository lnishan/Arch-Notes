# Arch-Notes
My short notes for [CMU 18-447 Introduction to Computer Architecture – Spring 2015](http://www.ece.cmu.edu/~ece447/s15/doku.php?id=schedule) (lectured by [Prof. Onur Mutlu](http://users.ece.cmu.edu/~omutlu/)).  
All the lecture materials (including lecture videos) are available on its [course page](http://www.ece.cmu.edu/~ece447/s15/doku.php?id=schedule).

## Lecture Notes

### L01. Introduction and Basics

- *Denial of memory service* (matlab vs gcc): cache locality, fairness problem, row buffer miss
- *DRAM refresh*: profile, more frequent refreshes for weaker rows
- Disturbance effects: all memories, aggressor/victim row, error correction mechanisms

### L02. Fundamental Concepts and ISA

- ![stack](http://i.imgur.com/VLOMeV1.png)
- Architecture today: every component is being reevaluated
- 3 key components: *Computation*, *Communication* and *Storage*
- Storage: *Memory* (non-persistent storage like DRAM, persistent storage like flash memory) and *Storage system* (emerging technologies getting closer to DRAMs).
- *Von Neumann model*: control flow order (specified by *instruction pointer*)
- *Dataflow model*: data flow order (fired when its *operands* are ready, no instruction pointer)
- Dataflow nodes: conditional (branching), relational, barrier synchronization (parallel programs)  
- *ISA*: Agreed upon interface between software and hardware
- *Microarchitecture*: a specific implementation of ISA, not visible to software
- *Microprocessor*: ISA, uarch, circuits
- *"Architecture"** = ISA + microarchitecture
- ISA = car functions (turn, acceleration/deceleration). Microarchitecture = how car manufacturers implement the functions underneath.
- ![ISA](http://i.imgur.com/M1TPhNV.png)

### L03. ISA Tradeoffs

- *Bit steering*: A bit to determine the type of instruction for interpretation
- Instruction: *opcode*, *operands*
- ISA elements:
    - Instruction sequencing model (control flow vs. data flow)
    - Instruction processing style (0, 1, 2, 3 address machines)
    - Instructions
    - Data types
    - Memory organization (Address space, Addressability)
    - Registers
    - Load/store (only on registers, RISC, ARM) vs. memory/memory architectures (CISC, x86)
- *Addressing modes*: how to describe memory address. More = better for programmers.
- *Orthogonal ISA*: (No. of addr modes) * (No. of opcodes) * (No. of data types)
- More ISA elements:
    - Privilege modes (permission)
    - Exception and interrupt handling
    - Virtual memory (virtual memory space > physical)
    - Access Protection
- CISC (Complex) vs. RISC (Reduced)

| Characteristics | CISC (x86) | RISC (ARM) |  
| --- | --- | --- |  
| Operates on | **Both** | Register only |  
| Addressing modes | **More** | Less |  
| Code size | **Shorter** | Longer |  
| Compiler Work | **Less** | More |  
| Optimization | Rougher | **Finer** |  
| Hardware | Complex | **Simpler** |  
| Semantic Gap | Smaller | Greater |  
| Instruction Length | Variable | Fixed |  
| Decode uniformity | Non-uniform | Uniform |

-  Number of registers: More => better utilization and optimization, larger instruction size (more bits for addr)


## License
[CC Attribution-Share Alike 3.0 Unported](http://creativecommons.org/licenses/by-sa/3.0/)

