# General Object Tracking #

## Methods in Tracking ##
From the last several years, with examples,
[tracking_solutions](https://docs.google.com/presentation/d/1Edcf8GrBHDkwU12HIXyqMXeEJvCQPmZQ6TsPfckypII/edit?usp=sharing):
<a href="https://docs.google.com/presentation/d/1Edcf8GrBHDkwU12HIXyqMXeEJvCQPmZQ6TsPfckypII/edit?usp=sharing">
  <img src="https://github.com/ilarele/tracking-paper-notes/blob/master/tracking_solutions_content.png" width="60%">
</a>


## Tracking Benchmarks ##
Classical and newer/larger datasets,
[tracking_benchmarks](https://docs.google.com/presentation/d/14TFUGZrk-nIQPy5t6hB07yBqN6ZEGgjL37j5uyfKsU0/edit?usp=sharing):
<a href="https://docs.google.com/presentation/d/14TFUGZrk-nIQPy5t6hB07yBqN6ZEGgjL37j5uyfKsU0/edit?usp=sharing">
<img src="https://github.com/ilarele/tracking-paper-notes/blob/master/tracking_benchmarks_content.png" width="60%">
</a>

## Results ##
Recent tracking solutions on those benchmarks,
[trackers_results](https://docs.google.com/spreadsheets/d/1JC-paakUZ4SEj6D2k8NktpiJ_c5G1DrZ2eah5oUzGgE/edit?usp=sharing):

| Tracker Name                   | FPS | TrackingNet testset | -       | LaSOT testset | -       | VOT'18 ST  | -        | -    | VOT'17 ST  | -        | -    | OTB50   | -         | OTB100  | -         | VOT'16 ST   | -        | -   | VOT'15 ST  | -        | -   | LaSOT all | -       | GOT-10k | -       | -    | TempleColor128 | NFS | UAV123 |
|--------------------------------|-----|---------------------|---------|---------------|---------|------------|----------|------|------------|----------|------|---------|-----------|---------|-----------|-------------|----------|-----|------------|----------|-----|-----------|---------|---------|---------|------|----------------|-----|--------|
|                                | GPU | NormPrec            | Success | NormPrec      | Success | Robustness | Accuracy | EAO  | Robustness | Accuracy | EAO  | Success | Precision | Success | Precision | Robustness  | Accuracy | EAO | Robustness | Accuracy | EAO | NormPrec  | Success | SR 0.5  | SR 0.75 | AO   | AUC            | AUC | AUC    |
| [ICCV'19] **DiMP-50**          | 43  | 68.7                | 74      | -             | 56.9    | 153        | 597      | 0.44 | -          | -        | -    | -       | -         | 68.4    | -         | -           | -        | -   | -          | -        | -   | -         | -       | 71.7    | 49.2    | 61.1 | -              | -   | -      |
| [ICCV'19] **DiMP-18**          | 57  | 66.6                | 72.3    | -             | 53.5    | 182        | 594      | 402  | -          | -        | -    | -       | -         | 66      | -         | -           | -        | -   | -          | -        | -   | -         | -       | 67.2    | 44.6    | 57.9 | -              | -   | -      |
| [CVPR'19] **ATOM**             | 30  | 77.1                | 70.3    | 57.6          | 51.5    | 204        | 0.59     | 401  | -          | -        | -    | -       | -         |         | -         | -           | -        | -   | -          | -        | -   | -         | -       | 63.4    |         | 55.6 | -              | 59  | 65     |
| [CVPR'19] **SiamRPN++**        | 35  | 80                  | 73.3    | 56.9          | 49.6    | 234        | 0.6      | 414  | -          | -        | -    | -       | -         | 69.6    | 914       | -           | -        | -   | -          | -        | -   | -         | -       | -       | -       | -    | -              | -   | 61.3   |
| [CVPR'19] **SPM**              | 120 | -                   | 71.2    | -             | 47.1    | -          | -        | -    | 0.3        | 0.58     | 338  | 65.3    | -         | 68.7    | -         | 0.21        | 0.62     | 434 | -          | -        | -   | -         | 48.5    | -       | -       | -    | -              | -   | -      |
| [CVPR'19] **C-RPN**            | 32  | 74.6                | 66.9    | -             | 45.5    | -          | -        | -    | -          | -        | 289  | -       | -         | -       | -         | 0.95        | 594      | 363 | -          | -        | -   | -         | 45.9    | -       | -       | -    | -              | -   | -      |
| [CVPR'19] **SiamMask**         | 55  | -                   | -       | -             | -       | 0.38       | 609      | 0.38 | -          | -        | -    | -       | -         | -       | -         | 214         | 639      | 433 | -          | -        | -   | -         | -       | -       | -       | -    | -              | -   | -      |
| [CVPR'19] **ASRCF**            | 28  | -                   | -       | -             | 35.9    |            |          |      | 234        | 494      | 328  | 69.2    | 922       | -       | -         | 187         | 563      | 391 | -          | -        | -   | -         |         | -       | -       | -    | -              | -   | -      |
| [CVPR'19] **SiamDW: SiamFC+**  | 70  | -                   | -       | -             | -       | -          | -        | -    | 0.49       | 0.5      | 0.23 | 67      | 0.88      | 64      | 0.85      | -           | -        | -   | -          | -        | -   | -         | -       | -       | -       | -    | -              | -   | -      |
| [CVPR'19] **SiamDW: SiamRPN+** | 150 | -                   | -       | -             | -       | -          | -        | -    | 0.41       | 0.52     | 0.3  | 67      | 0.92      | 67      | 0.9       | -           | -        | -   | -          | -        | -   | -         | -       | -       | -       | -    | -              | -   | -      |
| [CVPR'19] **GCT**              | 50  | -                   | -       | -             | -       | -          | -        | -    | -          | -        | 274  | 67      | 873       | 64.8    | 854       | -           | -        | -   | -          | -        | -   | -         | -       | -       | -       | -    | -              | -   | 50.8   |
| [CVPR'19] **UDT**              | 55  | -                   | -       | -             | -       | -          | -        | -    | -          | -        | -    | -       | -         | 63.2    | 80.6      | ?? 66 fails | 0.53     | 301 | -          | -        | -   | -         | -       | -       | -       | -    | -              | -   | -      |
| [CVPR'19] **TADT**             | 33  | -                   | -       | -             | -       | -          | -        | -    | -          | -        | -    | -       | -         | 68      | 0.66      | 1.17        | 0.55     | 299 | 1.09       | 0.59     | 327 | -         | -       | -       | -       | -    | 56.2           | -   | -      |
| [CVPR'19] **RPCF**             | 5   | -                   | -       | -             | -       | -          | -        | -    | 234        | 0.5      | 316  | 71.3    | 954       | 69      | 929       | -           | -        | -   | -          | -        | -   | -         | -       | -       | -       | -    | -              | -   | -      |
