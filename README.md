# CPU Benchmark

A minimal Docker image based on Ubuntu 22.04 for benchmarking CPU performance using sysbench.

## What's Inside

Base image: ubuntu:22.04

Benchmark tool: sysbench

Default command: Runs a CPU test using 2 threads.

## Usage

Run the container to execute a CPU benchmark test:

```bash
docker run --rm nomansadiq11/cpu-benchmark
```

You can customize the sysbench parameters by overriding the default CMD:

```bash
docker run --rm nomansadiq11/cpu-benchmark sysbench cpu --threads=4 --time=30 run
```

## Sample Output

```text
CPU speed:
    events per second: 12345.67

```

## Customize Thread Count

Change the number of threads to simulate different CPU loads:


```bash
docker run --rm nomansadiq11/cpu-benchmark sysbench cpu --threads=8 run
```
