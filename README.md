# Learnable-Fourier-Features

Unofficial PyTorch implementation of the paper "[Learnable Fourier Features for Multi-Dimensional Spatial Positional Encoding](https://arxiv.org/pdf/2106.02795.pdf)", NeurIPS 2021.


Basic usage is as below:
```python
from positional_encoding import LearnableFourierFeatures as LFF

lff = LFF(pos_dim=2, f_dim=128, h_dim=256, d_dim=64) # learnable fourier features module
pos = torch.randn([4, 1024, 1, 2])  # random positional coordinates
pe = lff(pos)  # forward

```

More detailed explanation of usage can be found in the file `positional_encoding.py`.

Other popular positional encoding methods such as the sinusoidal positional encoding from the paper "[Attention is All You Need](https://arxiv.org/pdf/1706.03762)", and fourier features from the paper "[Fourier Features Let Networks Learn High Frequency Functions in Low Dimensional Domains](https://arxiv.org/pdf/2006.10739)" are also implemented in the file.
