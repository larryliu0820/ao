## Autotuner and custom Triton kernels

### Use case

### How to contribute

### Environment variables

`TORCHAO_AUTOTUNER_ENABLE=0`

Set this to a nonzero value to enable the autotuner. This is turned off by default, because it is still an experimental feature.

`TORCHAO_AUTOTUNER_SEARCH=0`

Set this to a nonzero value to enable the search functionality of the autotuner for unseen shapes or on unknown hardware.

Searching a new config can take a long time and we'll save the updated data in `data.pkl`. If you'd like to contributed updated configs for your hardware or shapes, please open a pull request.

`TORCHAO_AUTOTUNER_DATA=torchao/kernel/configs/data_a100.pkl`

By default we load precomputed configs for A100. If we're not on an A100, we search set the path to `data.pkl`.