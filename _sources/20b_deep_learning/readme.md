# Segmentação de imagens baseada em Deep Learning

Neste capítulo, usaremos algoritmos baseados em deep learning para segmentação de imagens.

## Instalação dos requisitos

Para usar [cellpose](https://cellpose.readthedocs.io/) e [stardist](https://github.com/stardist/stardist), estas dependências devem ser instaladas:

```
mamba install cellpose pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts
pip install tensorflow
pip install stardist
```

Os notebooks nesta pasta foram testados usando
* `torch==2.0.1`
* `stardist==0.8.3`
* `tensorflow==2.12.0`
* `csbdeep==0.7.3`
* `cellpose==2.2.1`