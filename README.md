# FLAME GPU 2 Tutorial (Python 3)

This repository provides a Tutorial on using the Python 3 interface for [FLAME GPU 2](https://github.com/FLAMEGPU/FLAMEGPU2).

## Tutorial

The tutorial is a jupyter notebook which uses a predator-prey model to demonstrate how models can be described and implemented using FLAME GPU 2's python interface, and then simulated to observe population dynamics over the duration of a single simulation.

A number of exercises are presented to change and extend the behaviour of the model and observe the differences.
Solutions are provided.

## Instructor-led Tutorials

Instructor-led delivery of this tutorial will typically use hosted Jupyter solutions, such as cloud instances on [InstanceHub](https://www.instancehub.com/) or through [Google Colab](https://colab.research.google.com/).

Please refer to the instructions provided during by the instructor(s) on how to access the tutorial in this case.

If you are interested in an instructor-led delivery of this tutorial, please [contact us](https://flamegpu.com/contact/).

## Self-paced Tutorials

If you wish to follow this tutorial at your own pace, you can run this tutorial locally, or use a hosted service such as Google Colab.

This tutorial was previously delivered at:

+ 2021-09-08 [SeptembRSE 2021](https://septembrse.github.io/) [Workshop S1005: FLAME GPU 2: Complex Systems Simulation using GPUs](https://septembrse.github.io/#/event/S1005) 
  + Delivered by Paul Richmond, Matthew Leach, Peter Heywood and Robert Chisholm

### Google Colab

A Google Colab-based version of this tutorial will be made available in the future.

### Running this Tutorial Locally

> **Note**: The notebook currently assumes you are using python 3.6, with CUDA 11.0 on a Linux x86_64 machine. This will be corrected in the future.

To run this tutorial locally you will require:

+ Python `>= 3.6`
+ CUDA `>= 11.0` and a [Compute Capability](https://developer.nvidia.com/cuda-gpus) >= 3.5 NVIDIA GPU
+ Linux with `glibc >= 2.17`
  + Windows support/instructions will be introduced at a later date
+ An `x86_64` CPU
  + Including [`NVRTC`](https://docs.nvidia.com/cuda/nvrtc/index.html)
  + If you wish to run this tutorial on an `ppc64le` or `arm64-sbsa` based-system, you will need to build `pyflamegpu` from source.
  Please see the main [FLAMEGPU/FLAMEGPU2](https://github.com/FLAMEGPU/FLAMEGPU2) repository for instructions on building from source.

1. Clone the repository if you have not already done so

2. Create a new python `venv` or conda environment and activate it
  
    ```bash
    # I.e. if using a venv on linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3. [Install Jupyterlab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html) (or jupyter notebook)

    ```bash
    # I.e. if using a venv and pip
    python3 -m pip install -U jupyterlab
    ```

4. Launch `jupyter lab` or the legacy `jupyter notebook` interface and open `FLAME_GPU_2_python_tutorial.ipynb`

    ```bash
    # Using jupyter lab
    jupyter lab FLAME_GPU_2_python_tutorial.ipynb
    # Using jupyter notebook
    jupyter notebook FLAME_GPU_2_python_tutorial.ipynb
    ```
