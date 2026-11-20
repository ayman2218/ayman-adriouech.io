# Edge AI for automotive ECUs — PQK

**Focus:** Automotive embedded AI, compression, inference benchmarking, GTSRB.

## Project overview
This research-oriented case study combines **structured pruning (30%)**, **INT8 post-training quantization**, and **knowledge distillation (T=4, α=0.5)** for a YOLOv5-family model on traffic-sign classification.

## Reported experimental results
| Stage | Model size | Mean latency | Worst observed latency | Top-1 |
|---|---:|---:|---:|---:|
| Baseline FP32 | 65.0 MB | 45.2 ms | 52.1 ms | 94.2% |
| Structured pruning | 45.5 MB | 34.8 ms | 39.5 ms | 93.8% |
| INT8 quantization | 11.3 MB | 10.2 ms | 12.5 ms | 89.2% |
| PQK final | 12.0 MB | 8.3 ms | 10.1 ms | 92.5% |

The portfolio describes an **ARM Cortex-A53 (1.5 GHz, 512 MB RAM) emulation / modeled environment** and TensorFlow Lite. These are **project-reported values**, not independently verified measurements on a production ECU.

## Safety and limitations
ISO 26262, HARA, and ASIL are important engineering considerations, but **timing benchmarks alone do not establish ISO 26262 or ASIL B compliance**. Production qualification would require safety analyses, evidence, toolchain validation and system-level testing.

## Source availability
Technical documentation is based on the author's supplied portfolio. **Training scripts, trained weights and datasets have not been uploaded to this repository.** Please request them if available and suitable for public sharing.
