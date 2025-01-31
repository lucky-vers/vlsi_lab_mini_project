---
title: "IEEE 754 32-bit Floating Point Multiplier"
author:
  - Lakshit Verma (230959210)
  - Pranav Saini (230959212)
date: "January 31, 2025"
geometry: margin=3cm
...

# Abstract

Floating point arithmetic is widely used in various computing applications, including scientific computations, digital signal processing, and graphics processing. This project focuses on the design and implementation of an IEEE 754 compliant 32-bit floating point multiplier using VLSI design methodologies. The IEEE 754 standard defines a precise format for representing floating point numbers and ensures accuracy in floating point operations.

The implementation is carried out using Verilog HDL and synthesized using FPGA-based tools to evaluate the area, power, and timing performance.

The results demonstrate efficient multiplication with optimized resource utilization, making it suitable for high-performance computing applications. This mini-project provides insights into floating point arithmetic and its practical realization in VLSI circuits.

## IEEE 754 Format
A 32-bit floating-point number consists of three parts:

\begin{center}
\texttt{SEEEEEEE EMMMMMMM MMMMMMMM MMMMMMMM}
\end{center}

where:

- **`S` (1 bit)** → Sign bit (0 = positive, 1 = negative)

- **`E` (8 bits)** → Exponent (biased by 127)

- **`M` (23 bits)** → Mantissa (fraction part, normalized)

Let's take a sample 32-bit binary representation:

\begin{center}
\texttt{0 10000010 11000000000000000000000}
\end{center}

- **Sign bit (0)** → Positive number
- **Exponent (10000010 in binary = 130 in decimal)**
  Actual exponent = `130 - 127 = 3`
- **Mantissa (1.110 in binary = 1.75 in decimal, since implicit leading 1)**

Thus, the value is:

\begin{center}
$1.75 \times 2^3 = 14.0$
\end{center}

**Keywords**: IEEE 754, Floating Point Arithmetic, Multiplier, Verilog, VLSI, FPGA

