# DJ Track Session Manager: C++ Memory Management

This project is a C++ system that models a DJ track session manager while emphasizing **manual memory management** and **resource ownership**. It is designed as a learning-oriented codebase to practice safe and efficient handling of dynamic memory in modern C++ in the context of a realistic application domain (tracks, playlists, and DJ sessions).

## Technical Highlights

- **C++ Memory-Centric Design**: Every major component is structured to highlight dynamic allocation, RAII, copy/move semantics, and correct resource cleanup.
- **Session & Playlist Abstractions**: DJ sessions, playlists, and tracks are modeled with clear ownership relations to make lifetime and responsibility of objects explicit.
- **Resource Caching**: Certain components simulate caching of tracks/resources, providing a concrete context for practicing object lifetime management.
- **Leak-Free Execution Goal**: The architecture is intended to run without memory leaks or invalid frees, encouraging use of smart pointers and well-designed destructors.

## Tech Stack

- **Language**: C++ (modern standard, as required by the assignment).
- **Build Tool**: `Make` with a provided `Makefile`.
- **Environment**: Linux / WSL / University lab machines (as specified in the course).

## System Concept

The system follows a **DJ session management** logic:

1. **Track Management**: Audio-like entities (tracks) are created, stored, and referenced by playlists and sessions.
2. **Playlist & Session Flow**: Playlists group tracks, and sessions orchestrate the playback/order of these playlists.
3. **Memory & Ownership**: Each object has clear ownership rules (who allocates, who deletes, when copies/moves happen), forming the core of the assignment’s learning goals.

## Quick Start

From the project root (where the `Makefile` is located):

```bash
make           # build the project
./bin/dj_manager   # run the main executable (or the name defined in your Makefile)
```

If your assignment defines additional targets (such as `debug`, `release`, `test`, or memory-check targets), use them according to the course instructions.

---

### Professional Summary

**DJ Track Session Manager: C++ Memory Management** showcases the ability to design a small but realistic system that focuses on **memory safety**, **ownership semantics**, and **resource lifetime management**. It is a practical demonstration of how to embed low-level C++ concepts (allocation, deallocation, RAII, copy/move operations) inside a coherent application scenario, preparing you for larger-scale systems programming tasks. 