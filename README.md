# Quake-OpenMP
Parallel computing model for earthquake simulations

## Overview
This project implements a parallel computing model based on Loukas Kallivokas and David O'Hallaron's program to simulate earthquake wave propagation using a **sparse matrix-vector product (SMVP)** computation. The program is written in **C** and utilizes **OpenMP** parallel processing to enhance computational efficiency.

## Features
- Parallelized using **OpenMP** for shared memory systems.
- Simulates earthquake wave propagation using **sparse matrix-vector product (SMVP)**.
- Performance optimization via **loop parallelization and cache-friendly memory access**.

## Usage
### **Compilation**
Run the provided **Makefile** to compile the program:
```sh
gcc -fopenmp -o quake quake_omp.c -lm
```

### **Running the Program**
Run the program with customizable simulation parameters:
```sh
./quake << quake.in
```

## Performance
The program achieves significant speedup by leveraging **OpenMP parallelization** for multi-core CPUs.
![alt text](https://github.com/hellojoel/Quake-OpenMP/blob/main/perfplot.png?raw=true)


## References
- OpenMP Documentation: https://www.openmp.org/
- Seismic Wave Propagation Models

