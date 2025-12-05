# Elastic Nano-vLLM
## Nano-vLLM
What is Nano-vLLM?     
A lightweight vLLM implementation built from scratch.

Key Features:
- * 🚀 **Fast offline inference** - Comparable inference speeds to vLLM
- * 📖 **Readable codebase** - Clean implementation in ~ 1,200 lines of Python code
- * ⚡ **Optimization Suite** - Prefix caching, Tensor Parallelism, Torch compilation, CUDA graph, etc.


## Installation
First, install nano-vLLM using pip:
```bash
# Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate
# torch
pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu128
# FlashAttention
wget https://github.com/Dao-AILab/flash-attention/releases/download/v2.8.1/flash_attn-2.8.1+cu12torch2.9cxx11abiTRUE-cp312-cp312-linux_x86_64.whl
pip install flash_attn-2.8.1+cu12torch2.9cxx11abiTRUE-cp312-cp312-linux_x86_64.whl
# nano-vLLM
pip install git+https://github.com/GeeeekExplorer/nano-vllm.git
```
Download model weights from Hugging Face:
```bash
export HF_ENDPOINT=https://hf-mirror.com
huggingface-cli download --resume-download Qwen/Qwen3-0.6B --local-dir-use-symlinks False --force-download
```



