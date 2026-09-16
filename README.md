# ISC26 DFTB+ Working Copy

This repository is a working copy of the upstream [DFTB+](https://github.com/dftbplus/dftbplus) project that I used for ISC26 competition experiments.

It does not represent original authorship or maintenance of the DFTB+ codebase. The upstream project and its contributors remain the source of the underlying implementation.

## My ISC26 modification

My competition-specific change is preserved on the [`isc26`](https://github.com/YuTingChen0502/isc26-dftbplus/tree/isc26) branch in commit [`0cf095c`](https://github.com/YuTingChen0502/isc26-dftbplus/commit/0cf095c8defab8c994a6d55149c05b2162238388).

The patch removes the `OMP_THREADS == 1` restriction from selected ELSI-related test conditions and removes the corresponding manual warning, allowing experiments with multi-threaded ELSI configurations in this working copy.

Changed areas:

- ELSI-related test-selection constraints under `test/app/dftb+/tests`
- the corresponding ELSI/OpenMP warning in `doc/dftb+/manual/dftbp.tex`

## Scope

The patch is an experimental competition modification. By itself, it does not establish that every ELSI solver is correct, stable, or faster with multiple OpenMP threads.

This repository is retained primarily as provenance for the ISC26 experiment rather than as a standalone DFTB+ project.

## Upstream

For the maintained DFTB+ codebase, documentation, issues, and releases, use the upstream repository:

- https://github.com/dftbplus/dftbplus
