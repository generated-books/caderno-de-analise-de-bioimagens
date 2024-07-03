# Deconvolução de imagem
A deconvolução de imagem é também _apenas_ uma forma especial de filtragem de imagem. Dedicamos um capítulo inteiro a isso porque as deconvoluções desempenham um papel importante na microscopia de fluorescência.

Demonstraremos os princípios em imagens bidimensionais. No entanto, deve-se destacar que a deconvolução deve ser feita em três dimensões, se possível, porque os princípios físicos subjacentes não são os mesmos em todas as direções, a função de espalhamento de ponto normalmente não é simétrica na microscopia de fluorescência.

## Instalando os requisitos

Usaremos [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish) e [SimpleITK](https://simpleitk.readthedocs.io/) para deconvolver imagens. Para facilitar o uso, trabalharemos com o último através de uma camada de conveniência, [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing). Digite estes comandos no terminal para instalar tudo:

```
mamba install reikna pyopencl -c conda-forge
pip install redlionfish
pip install napari-simpleitk-image-processing
```

<!--
## Instalando dependências opcionais

Em um notebook, também usaremos NVidia CUDA para deconvolução. Se sua unidade de processamento gráfico suportar cuda, fique à vontade para instalar [pycudadecon](https://github.com/tlambert03/pycudadecon).

```
mamba install -c conda-forge pycudadecon
```
-->

## Veja também
* [BioDIP Dresden, Como deconvolver imagens usando Huygens](https://www.biodip.de/wiki/How_to_deconvolve_images_using_Huygens)