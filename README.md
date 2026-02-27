# CNRS/IDRIS HPC Self-Study 🚀

**Official training materials from IDRIS (CNRS supercomputing institute)** 
[Training materials](https://www.idris.fr/eng/formations/supports_de_cours-eng.html)

Self-directed study of official training materials from IDRIS (CNRS supercomputing center), focused on scalable scientific computing for plasma physics applications.
If access to the Jean Zay supercomputer is available, experiments will be conducted there.  
Otherwise, all exercises will be benchmarked on local or alternative HPC resources with full hardware documentation.

---

## Objective

Develop practical HPC expertise applicable to:

- Particle-in-Cell (PIC) simulations  
- Tokamak-scale PDE solvers  
- Hybrid CPU/GPU architectures  
- Performance engineering & scalability analysis  

This repository documents exercises, implementations, benchmarks, and performance studies completed during this training.

---

## Timeline (March – April 2026)

Training starts: **Early March 2026**  
Target completion: **End of April 2026**

The schedule accounts for academic exams and coursework constraints.

---

## Training Structure

The training follows a progressive path from shared-memory parallelism to GPU acceleration and performance engineering.

---

### Phase 1 — Shared Memory & Hybrid Parallelism (March)

| Module | Focus | Status |
|--------|-------|--------|
| Hybrid MPI + OpenMP | Poisson3D hybridization, scaling | In progress |
| OpenMP | Loops, tasks, affinity, scheduling | Planned |

**Planned outputs**
- Strong scaling study
- Weak scaling study
- Thread affinity experiments
- Pure MPI vs Pure OpenMP vs Hybrid comparison

---

### Phase 2 — Distributed Memory (Late March)

| Module | Focus | Status |
|--------|-------|--------|
| MPI Fundamentals | Point-to-point, collectives | Planned |
| Advanced MPI | Non-blocking communication, Cartesian grids | Planned |

**Applied project**
- 2D domain decomposition  
- Halo exchange optimization
- Communication/computation overlap  

---

### Phase 3 — GPU Acceleration (April)

| Module | Focus | Status |
|--------|-------|--------|
| OpenACC | Kernel offloading | Planned |
| GPU Optimization | Memory transfers, async execution | Planned |

**Applied to plasma physics**
- GPU-accelerated Boris particle pusher
- Parallel reduction optimization
- CPU vs GPU benchmarking

---

### Phase 4 — Performance Engineering (April)

Tools and methodologies:

- perf  
- VTune  
- Nsight  
- Roofline analysis  
- Memory bandwidth diagnostics  
- Cache blocking & vectorization

Final deliverable:
- `rapport.pdf` including scaling curves, bottleneck analysis, and optimization iterations.

---

## Applications to Fusion Plasma Simulation

This training is oriented toward computational challenges found in:

- Particle-in-Cell (PIC) codes  
- MHD solvers  
- Global tokamak simulations  
- Hybrid CPU+GPU architectures  

Key topics explored:

- GPU particle push (Boris method)  
- Domain decomposition strategies  
- Strong-scaling limits  
- Memory-bound vs compute-bound regimes  

---

## Hardware Policy

Each benchmark will include:

- CPU/GPU model  
- Core/thread count  
- Memory configuration  
- Compiler and flags  
- Runtime configuration  

If access to Jean Zay is obtained, dedicated scaling studies will be added.

Otherwise, equivalent methodology will be applied on available hardware.

---

## Benchmarking Philosophy

Each completed exercise will include:

- Hardware specification  
- Compilation flags  
- Scaling plots  
- Parallel efficiency analysis  
- Identified bottlenecks  
- Optimization attempts  

Reproducibility and clarity are prioritized.

---

## Milestones (2026)

- [ ] Hybrid Poisson3D TP — Mid March  
- [ ] MPI domain decomposition — Late March  
- [ ] GPU Boris pusher benchmark — Mid April  
- [ ] Performance engineering report — End April  

---

## Repository Structure (to be expanded)

/hybrid_mpi_openmp/
/mpi_domain_decomposition/
/openacc_gpu/
/benchmarks/
/report/

Each module will contain:
- Source code  
- Build instructions  
- Execution scripts  
- Benchmark results  
- Technical notes  

---

## Long-Term Goal

Build a rigorous HPC portfolio aligned with:

- Fusion research laboratories  
- Supercomputing centers  
- Industrial fusion startups  
- Large-scale plasma simulation development  

---

## Status

Training begins March 2026.  
Repository will be updated progressively as exercises are completed and optimized.

---
![CNRS-IDRIS](https://img.shields.io/badge/CNRS-IDRIS-00AEEF?style=flat&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAiIGhlaWdodD0iMTAiPjwvc3ZnPg==)
![Jean Zay](https://img.shields.io/badge/Jean_Zay-Supercomputer-orange)
