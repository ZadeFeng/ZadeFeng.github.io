---
title: "Technical Overview: Low-Level Programming for an Embedded GBA Game"
excerpt: "A technical deep dive into the architecture and low-level optimizations of the GBA puzzle game I built in C, focusing on memory management with DMA and interrupt-driven input. <br/><img src='/images/gba-project-teaser.png'>"
collection: portfolio
author_profile: true
---

**Project:** "Ink Link" - A Puzzle Game for the Game Boy Advance (GBA)  

### Introduction

The goal of this project was to develop a complete, playable puzzle game in C for a Game Boy Advance (GBA) emulator. The primary challenge was engineering a real-time application within a severely resource-constrained environment (2.24 MHz ARM7TDMI CPU, 256KB EWRAM). The focus was on achieving a consistent 60 FPS through low-level hardware manipulation and optimization.

### System Architecture

The game's architecture was designed around direct hardware access, as there was no operating system. The core components included a central game loop, an interrupt-driven input handler, game state update logic, and a rendering engine that wrote pixel data directly to video memory via memory-mapped I/O.



### Core Technical Challenge: Performance Optimization

##### **Memory Management with Direct Memory Access (DMA)**
The most significant performance bottleneck was memory copying. Relying on the CPU for tasks like clearing the screen or loading sprites would consume valuable cycles.

**Solution:** I utilized the GBA's **Direct Memory Access (DMA)** controller to offload large memory copy operations to dedicated hardware, allowing the CPU to execute game logic in parallel.
