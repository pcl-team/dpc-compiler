---
theme: metropolis
title: DPC++
subtitle: Suggested Projects
author: 'Ahmed El-Mahdy'
institute: 'E-JUST'
date: 16 April 2020
toc: false
slide_level: 2
header-includes: \metroset{progressbar=frametitle,sectionpage=progressbar}
---

# DPC++ lite for embedded devices

## Concept 

- Develop a backend for the Intel DPC++ for targetting embedded GPUs.
- The backend would consider earlier research conducted at E-JUST for reverse engineering the texture cache hierarchy.
- This would provide for cache aware optimisation, potentially allowing for up to $4\times$ performance improvement.

# Translating Binaries into DPC++

## Concept 

- The concept here is to convert legacy binaries written in CUDA into DPC++.
- The rationale here is the allow for porting existing CUDA programs where the source code of which is not avaliable.

# DBT: Dynamic Binary Parallelisation into DPC++

## Concept 

- Many programs are legcy programs that require both parallelisation and maintainability.
- Usually binary codes are the only avaliable source.
- The aim here is to extend our proof-of-concept DBT work to generate parallel code automatically for GPUs.
- The GPU kernel code would be generated into DPC++, which can be manually further optimised

# Deep Learning Based Retargtability Optimiser for DPC++

## Concept 

- The main concept here is to utilise program models and Deep Learning, to learn code patterns for the GPUs.
- This has the potential to generate novel optimisation than just figure out optimisation parameter as per typical use of machine learning.
- The system would generate DPC++ code allowing for further optimisations.

## Related Work

- Probabilistic program model attempts of model, statistically, program patterns.
- This is currently used in analysis and synthesis of programs.
- No attempts has been yet done in the area of automatic parallelisation.

# Transpilers: (Restructing Compilers)

## Concept

- I couldn't find the source code of the Intel compatiblity tool.
- We propose of have a restructuring compiler that targets:
  - OpenMP
  - OpenACC
  - OpenCL
  - CUDA
  - Java?
  - Fortran?

## {.standout}

Thank you!


