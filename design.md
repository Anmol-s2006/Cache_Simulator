# Design and Implementation of a Configurable Cache Simulator for Memory Hierarchy Analysis

## Abstract

Modern CPUs rely heavily on cache performance; this project develops a simulator which is supposed to mimic the behavior of a hardware cache subsystem. This simulator is written in C language, due to it being an optimal choice between convenience and control.

The goal of this project is to simulate and analyze the effects of cache parameters on hit/miss performance and to explore the trade-offs in memory hierarchy design. 

## Introduction

### What is Cache ?

A cache is a small, fast storage device that acts as a staging area for the data objects in a larger, slower device. Caches are orders of magnitude faster than DRAM and as such are very important for speeding the overall operation of CPU without making CPU wait.

### Purpose of simulator 

A cache simulator is a valuable tool for computer architecture for several reasons:
    1. Performance Analysis
    2. Optimization of programs
    3. Explore different type of design.

### Some helpful definitions 

**Cache Hits** :- When a program needs a particular data object `d` from level `k+1`, it first looks for d in one of the blocks currently stored at level `k`. If `d` happens to be cached at level `k`, then that act is called cache hit.

**Cache Miss** :- If not found on level `k` then it is said as cache miss.

### Dimensions of Cache Design

