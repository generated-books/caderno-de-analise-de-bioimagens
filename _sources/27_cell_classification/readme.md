# Classificação de células

Para classificar objetos como células e núcleos, um procedimento comum é usar extração de características e, posteriormente, algoritmos de aprendizado de máquina, como Classificadores de Floresta Aleatória (Random Forest Classifiers), para diferenciar os objetos.

## Instalação das bibliotecas necessárias

Nesta seção, trabalharemos com [scikit-learn](https://scikit-learn.org) e [aopc](https://github.com/haesleinhuepf/apoc). Esses dois podem ser instalados da seguinte forma:

```
pip install scikit-learn
```

```
conda install -c conda-forge pyopencl
pip install apoc
```