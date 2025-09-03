# free-hours-experiments
Here I am collecting Jupyter notebooks with Linear Algebra, LLM whatever experiments, excercises... 

## Projects' Structures Overview

- **cuda_kernels/**
  - `softmax_normalizer_calculation_parallel.ipynb`: Jupyter notebook for parallel softmax normalization.
  - **tgautam03_xGeMM/**: CUDA-based matrix multiplication experiments.
    - `Makefile`: Build instructions.
    - `readme.md`: Subproject documentation.
    - **build/**: (Build outputs, if any.)
    - **include/**: CUDA headers
      - `01_naive_xgemm.cuh`, `02_coalesced_xgemm.cuh`, `MatrixFP32.cuh`, `utils.cuh`
    - **src/**: CUDA source files
      - `01_naive_xgemm.cu`, `02_coalesced_xgemm.cu`, `utils.cu`
    - **test/**: Benchmarks and tests
      - `00a_benchmark_cpu.cpp`, `00b_benchmark_cuBLAS.cu`, `01_benchmark_naive.cu`, `02_benchmark_coalesced.cu`

- **graphs/**
  - `Math_misconcept_graphs.ipynb`: Notebook for visualizing mathematical misconceptions and graph similarity metrics calculation.

- **kaggle/**
  - **lit_summaries_2023/**: Literature summary notebook
    - `set_fit.ipynb`
  - **otto/**: Kaggle competition pipeline for reatailer OTTO dataset using Tr4rec
    - `Transformers4Recs_Pipeline.ipynb`

- **linear_algebra/**
  - `Matrix_action_on_vectors.ipynb`: Notebook on matrix operations. Inspired by [Transformers without Normalization](https://arxiv.org/pdf/2503.10622)

- **optimal_transport/**
  - `Flow_Match.ipynb`: Notebook on flow matching algorithms.
  - `Sinkhorn_Algorithm.ipynb`: Notebook on Sinkhorn algorithm for optimal transport.

- **optimizers/**
  - `muon_newton_schultz.ipynb`: Notebook on Muon Newton-Schultz optimization.