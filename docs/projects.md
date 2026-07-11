# Current Major Projects

## MASIC

MASIC is my flagship engineering project: a complete computer architecture designed entirely from scratch for educational purposes, from the instruction set architecture to the physical hardware implementation and software toolchain. Development began in 2022 and concluded in 2026, representing four years of continuous design, implementation and refinement. MASIC was developed as my Bachelor's Thesis in Computer Engineering.

The project is centered around an original 8-bit accumulator-based CPU featuring a custom 16-bit address space, a microprogrammed control unit and a carefully designed instruction set focused on simplicity, consistency and educational value.

The complete architecture was designed from first principles and includes:

* Custom 8-bit accumulator-based CPU.
* Original Instruction Set Architecture (ISA).
* Microprogrammed control unit.
* 16-bit program counter and stack pointer.
* 64 KiB of main memory.
* Independent 64 KiB I/O address space.
* Nested interrupt system with a peripheral-supplied interrupt vector.
* Multiple addressing modes, including indirect addressing and stack-relative addressing.
* Complete stack architecture supporting subroutines and interrupts.
* Carefully designed instruction encoding with fixed instruction formats.
* Little-endian memory organization.

MASIC is part of a broader ecosystem that also includes dedicated software development tools and supporting hardware.

The processor architecture is complemented by a standalone video display adapter, the EMASIC cross macro assembler and the QTMASIC emulator, each developed as an independent project while maintaining complete architectural consistency across the ecosystem.

Instead of relying on programmable logic devices, the computer is implemented using low-scale integration with 74HC-series logic integrated circuits, allowing every subsystem to be understood directly at the hardware level. This approach was intentionally chosen to make every architectural component directly observable and understandable at the hardware level.

The project was conceived to demonstrate how an entire computer system can be designed from first principles while maintaining architectural consistency across hardware, firmware and software tools.

## EMASIC Cross Macro Assembler

EMASIC is a standalone cross macro assembler developed specifically for the MASIC architecture.

It was designed as a complete development tool rather than a simple assembler, providing a modern assembly workflow while remaining faithful to the educational goals of the architecture.

Its main features include:

* Cross assembly from modern desktop systems.
* Monolithic cross macro assembler implemented as a standalone native application.
* Powerful macro system supporting parameterized and nested macros.
* Local labels within macros with automatic unique symbol generation.
* Symbol resolution and expression evaluation.
* Support for complex compile-time arithmetic expressions.
* Multiple assembler directives for memory layout and data definition.
* Generation of flat binary executables.
* Comprehensive diagnostics and error reporting.

EMASIC was developed together with the ISA itself, allowing the instruction set, assembler syntax and software toolchain to evolve consistently throughout the design process.

The project demonstrates compiler front-end design, language parsing, symbol management and low-level software tooling.

## QTMASIC Emulator

QTMASIC is a desktop emulator developed specifically for the MASIC architecture.

Beyond functional emulation, it was designed as an educational debugging environment that allows software execution to be observed at multiple abstraction levels.

The emulator provides:

* Complete execution of MASIC machine code.
* Interactive debugging facilities.
* Register inspection.
* Memory visualization.
* Instruction-level execution.
* Signal-level simulation of the processor.
* Observation of the internal CPU state during execution.
* Integrated development workflow together with EMASIC.

Signal-level emulation allows the internal behaviour of the processor to be studied in detail, making the emulator useful not only for software development but also for validating the hardware architecture and understanding processor operation.

QTMASIC plays an important role within the MASIC ecosystem by bridging software development and hardware verification.

## Video Display Adapter

The video display adapter is an independent hardware subsystem developed specifically for MASIC.

Rather than integrating video generation into the CPU board, the display controller is implemented as a dedicated standalone expansion board built entirely with 74HC-series logic integrated circuits.

The CPU and the video subsystem communicate through a custom hardware interface that was also designed as part of the project, providing a clean separation between computation and display hardware while closely resembling the organization of real computer systems.

The video adapter required the design of digital video generation logic, timing circuitry, memory interfacing, synchronization mechanisms and system integration, making it a complete hardware project in its own right rather than simply an output peripheral.

This modular approach demonstrates the design of independent hardware subsystems connected through well-defined interfaces, reinforcing the educational and architectural goals of MASIC.

## ASMTRIS

ASMTRIS is a complete implementation of the classic Tetris game written entirely in Intel 8086 assembly language.

It was developed in 2022 as a personal project to deepen my understanding of x86 assembly programming, low-level software development and direct interaction with PC hardware through BIOS services.

The project intentionally relies exclusively on BIOS interrupt calls, without using external libraries, game engines or operating system APIs beyond the standard BIOS interface.

The implementation includes:

* Complete gameplay mechanics.
* Keyboard input handling through BIOS services.
* Video output using BIOS routines.
* Timing and game loop management.
* Collision detection.
* Piece rotation and movement logic.
* Line clearing and score management.
* Structured and modular assembly source code.

Although originally developed as a personal exploratory project, ASMTRIS became an excellent exercise in low-level programming, requiring careful management of registers, memory, control flow and performance within the constraints of the Intel 8086 architecture.

This project represents the beginning of my long-term interest in computer architecture and systems programming, eventually leading to the design and implementation of my own computer architecture, MASIC.

## FPGA Development

I have experience developing digital hardware in VHDL using Xilinx Vivado, gained through university projects and coursework.

My objective is to continue expanding my experience in FPGA-based processor implementation, building on the architectural knowledge acquired through the design of complete computer systems using discrete 74HC-series logic.

My long-term objective is to design processors and digital systems for FPGA and ASIC platforms, combining computer architecture, digital logic design and hardware/software co-design.

## Hardware Design Experience

Through MASIC I have gained practical experience in:

- Digital logic design using 74HC-series integrated circuits.
- CPU datapath design.
- Microprogrammed control unit design.
- Bus architecture.
- Interrupt controller design.
- Video generation hardware.
- Hardware/software co-design.
- System integration.
- Hardware debugging and validation.

## Portfolio Goals

The website should communicate:

Passion for computer architecture
Strong engineering mindset
Ability to design complete computing systems from scratch
Experience spanning both hardware and low-level software
Long-term commitment to processor and digital system design

Rather than presenting isolated projects, the portfolio should tell the story of my progression as an engineer.
