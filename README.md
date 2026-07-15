# ReFrame HPC/AI Test Suite

This repository collects ReFrame tests selected from open community test suites and adapts the applicable ones for HPC and AI cluster validation.

The goal is to reuse proven checks where possible instead of rebuilding common coverage from scratch. Initial review focuses on tests useful for AI infrastructure clusters: GPU runtime and burn-in checks, NCCL/RCCL and MPI communication, PyTorch smoke and distributed-training checks, scheduler/job-launch validation, container runtime checks, filesystem I/O, and representative HPC/AI application benchmarks.

## Source Test Suites Reviewed

| Organization | Repository | Focus |
| --- | --- | --- |
| CSCS | https://github.com/eth-cscs/cscs-reframe-tests | Applications, compilers, CUDA, I/O, system checks |
| EPCC / ARCHER2 | https://github.com/EPCCed/epcc-reframe | ARCHER2 and Cirrus synthetic and application benchmarks |
| Pawsey | https://github.com/PawseySC/Reframe-MPI-Stress-Tests | MPI stress, SLURM, GPU, software stack checks |
| CARC / USC | https://github.com/uschpc/reframe-tests | Modules, MPI, CUDA, Python/R/Julia, containers, I/O |
| HPC2N + C3SE | https://github.com/hpc2n/hpc2n-reframe-tests | Maintenance-tagged checks and multi-partition tests |
| VUB-HPC | https://github.com/vub-hpc/reframe-tests | OSU MPI, GROMACS GPU, SLURM, weekly checks |
| KAUST | https://github.com/kaust-rccl/ksl_postmaint_tests | Post-maintenance checks |
| ExCALIBUR | https://github.com/ukri-excalibur/excalibur-tests | Multi-system UK HPC benchmarks and Spack workflows |
| EESSI | https://github.com/EESSI/test-suite | Portable software installation and application testing |
| SKA Observatory | https://gitlab.com/ska-telescope/sdp/ska-sdp-benchmark-tests | Kernel, workflow, and pipeline benchmarks |
| StackHPC | https://github.com/stackhpc/hpc-tests | HPL, GROMACS, CP2K, WRF, OSU, IB/RoCE-oriented tests |
| Cineca | https://gitlab.hpc.cineca.it/mredenti/cineca-reframe | National HPC center ReFrame tests |

## Review Notes

The first static review of the open suites is in [docs/review/open-testsuites-review.md](docs/review/open-testsuites-review.md).

The review was generated from local clones using static parsing only. No ReFrame tests were imported or executed during the inventory pass.
