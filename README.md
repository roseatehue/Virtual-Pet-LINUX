Linux-Based Hardware-Integrated Virtual Pet System

A Tamagotchi-inspired virtual pet built using a microcontroller and a Linux-based system, demonstrating practical Operating Systems concepts through hardware and software integration.

Overview

This project aims to recreate the experience of having a virtual pet through a small physical device. Users will be able to interact with their pet using physical buttons, view its status on a display, and receive audio feedback.

Unlike a conventional virtual pet application, the core logic of this system will run as a multithreaded Linux process. A microcontroller will handle hardware interactions, while Linux will manage the pet's state, background updates, and data persistence.

Planned Features

- Interactive virtual pet with hunger, happiness, and fun statistics.
- Physical buttons for navigating menus and interacting with the pet.
- LCD/OLED display for showing the pet's status.
- Buzzer for audio feedback.
- Background updates to pet statistics over time.
- Persistent pet state across application restarts.
- Recovery of saved data after unexpected termination.

System Architecture

The system will consist of two main components:

1. Hardware Layer (Arduino/ESP32)

- Reads physical button inputs.
- Controls the display.
- Produces audio feedback.
- Communicates with the Linux system through USB serial communication.

2. Linux Software Layer

- Runs the main virtual pet program in C.
- Manages pet statistics and user interactions.
- Handles concurrent operations.
- Saves and restores pet data.

Operating Systems Concepts

The project aims to implement the following concepts:

Concept| Application
Multithreading| Handling user interactions and background stat updates.
Thread Synchronization| Using mutex locks to protect shared pet data.
I/O Multiplexing| Using "poll()" for serial communication.
File System and Persistence| Saving and restoring pet statistics.
Process Management| Managing the Linux pet process.
Crash Recovery| Protecting saved data against unexpected termination.

Technologies

- C
- Linux (Ubuntu)
- Arduino / ESP32
- POSIX Threads (pthreads)
- USB Serial Communication
- Git and GitHub

Development Status

Status: Planning / Initial Development

This project is currently under development. Features, implementation details, and documentation will be updated as development progresses.
