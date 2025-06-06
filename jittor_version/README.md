# One Prompt One Story (Jittor Version)

This is the Jittor implementation version of `One Prompt One Story`, Using the Jittor version of inference for SDXL in fp32 precision。
We refer to [this url](https://github.com/NK-JittorCV/nk-diffusion) for environment setup.

## Environment setup.

The Work is based on:

- [jittor](https://github.com/JittorRepos/jittor)
- [jtorch](https://github.com/JittorRepos/jtorch)
- [diffusers_jittor](https://github.com/JittorRepos/diffusers_jittor)
- [transformers_jittor](https://github.com/JittorRepos/transformers_jittor)

### 0. Clone JDiffusion & Prepare Env

```bash
git clone https://github.com/JittorRepos/JDiffusion.git
#We recommend using conda to configure the Python environment.
conda create -n jdiffusion python=3.9
conda activate jdiffusion
```

### 1. Install Requirements

Our code is based on JTorch, a high-performance dynamically compiled deep learning framework fully compatible with the PyTorch interface, please install our version of library.

```bash
pip install git+https://github.com/JittorRepos/jittor
pip install git+https://github.com/JittorRepos/jtorch
pip install git+https://github.com/JittorRepos/diffusers_jittor
pip install git+https://github.com/JittorRepos/transformers_jittor
pip install opencv-python scipy gradio==4.44.1 sympy==1.13.1
```

### 2. Install JDiffusion

```bash
cd JDiffusion
pip install -e .
```

More environment setup details please see [this url](https://github.com/NK-JittorCV/nk-diffusion)

## Quick Start
- Execute
```shell
conda activate jdiffusion
python python -m jittor_version.main
```

The demo experiment was conducted on a NVIDIA-3090 GPU.
