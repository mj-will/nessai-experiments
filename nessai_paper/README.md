# Nested sampling with normalising flows for gravitational-wave inference

[![arXiv](https://img.shields.io/badge/arXiv-1234.56789-b31b1b.svg)](https://arxiv.org/abs/2102.11056)

Code to reproduce the experiments described in [Nested sampling with normalising flows for gravitational-wave inference](https://doi.org/10.1103/PhysRevD.103.103006).

**Important:** these scripts are designed for use with `nessai==0.2.0`, `bilby==1.0.2`, and `bilby_pipe==1.0.3` and may not work with later versions.

**Important:** the settings used here reflect those used in the paper and no longer the recommended settings.

## Details

All ini files can be submitted by running:

```bash
bilby_pipe <name>.ini --submit
```

### P-P tests

The ini files that start `bbh_*` are for the P-P tests.

**Warning:** some of these runs can take more than a week to complete.

### Log-evidence distribution

The ini file labelled `log_z_dist_nessai.ini` submits 50 parallel runs with different seed that can be used to produce figure 4.

### Parallelisation

The ini file labelled `n_pool_nessai.ini` was used to produce figure 4.7.  The different runs were submitted by manually changing the label and `request-cpus`.
