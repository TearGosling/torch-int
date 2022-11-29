# torch-int
Integer operators for PyTorch

## Dependencies
- Cutlass
- PyTorch with CUDA 11.3
- Nvidia-Toolkit 11.3
- Cuda 11.3
- gcc g++ 9.4.0

## Installation
```bash
conda create -n int python
conda activate int
conda install -c anaconda gxx_linux-64=9
pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 torchaudio==0.12.1 --extra-index-url https://download.pytorch.org/whl/cu113
pip install -r requirements.txt
source environment.sh
bash build_cutlass.sh
python setup.py install
```

## Test
```bash
python tests/test_opt_decoder.py
```