# Arch-Notes
This a repo housing my short notes for [CMU 18-447 Computer Architecture – Fall 2015](http://www.ece.cmu.edu/~ece447/s15/doku.php?id=schedule) (lectured by [Prof. Onur Mutlu](http://users.ece.cmu.edu/~omutlu/)).  
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
- Dataflow nodes: Conditional (branching), Relational, Barrier synchronization (parallel programs)  
( FPGAs ? )
- *ISA*: Agreed upon interface between software and hardware
- *Microarchitecture*: A specific implementation of ISA, not visible to software
- *Microprocessor*: ISA, uarch, circuits
- *"Architecture"** = ISA + microarchitecture
- ISA = Car functions (turn, acceleration/deceleration). Microarchitecture = How car manufacturers implement the functions underneath.
- ![ISA](http://i.imgur.com/M1TPhNV.png)