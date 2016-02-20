# Arch-Notes
This a repo housing my short notes for [CMU 18-740 Computer Architecture – Fall 2015](http://www.ece.cmu.edu/~ece740/f15/doku.php).  
The lecture videos are openly available on [YouTube](https://www.youtube.com/playlist?list=PL5PHm2jkkXmi5CxxI7b3JCL1TWybTDtKq).

## Lecture Notes

### L01. Introduction and Basics

- denial of memory service (matlab vs gcc): cache locality, fairness problem, row buffer miss
- DRAM refresh: profile, more frequent refreshes for weaker rows
- disturbance effects: all memories, aggressor/victim row, error correction mechanisms

### L02. Fundamental Concepts and ISA

- ![stack](http://i.imgur.com/VLOMeV1.png)
- architecture today: every component is being reevaluated
- 3 key components: computation, communication and storage
- storage: memory (nonpersistent storage like DRAM, persisten storage like flash memory) and storage system (emerging technologies getting closer to DRAMs).
- Von Neumann model: control flow order (specified by instruction pointer)
- Dataflow model: data flow order (fired when its operands are ready, no instruction pointer)
- Dataflow nodes: conditional (branching), relational, barrier synchronization (parallel programs)
*FPGAs ?*
- ISA: Agreed upon interface between software and hardware
- Microarchitecture: A specific implementation of ISA, not visible to software
- Microprocessor: ISA, uarch, circuits
- "architecture" = ISA + microarchitecture
- ISA = car functions (turn, acceleration/deceleration). Microarchitecture = how car manufacturers implement the functions underneath.
- ![ISA](http://i.imgur.com/M1TPhNV.png)