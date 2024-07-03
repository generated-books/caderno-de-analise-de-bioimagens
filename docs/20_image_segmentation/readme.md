# Segmentação de imagem

Analistas de imagem referem-se à segmentação de imagem ao subdividir uma imagem em múltiplos grupos de pixels com características diferentes. Neste capítulo, aprenderemos algoritmos básicos para binarizar imagens e para rotular objetos em imagens.

## Instalação de requisitos

Assim como nos capítulos anteriores, usaremos [scikit-image](https://scikit-image.org/), [pyclesperanto-prototype](https://github.com/clEsperanto/pyclesperanto_prototype) e [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing) para segmentar as imagens. Algumas visualizações serão novamente feitas usando [matplotlib](https://matplotlib.org/).

## Instalação de dependências opcionais

Para alguns atalhos para algoritmos de segmentação de imagem baseados em watershed, recomenda-se a instalação do plugin scriptável napari [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes). Você pode instalá-lo usando pip:

```
pip install napari-segment-blobs-and-things-with-membranes
```

Veja também
* [Notebooks SimpleITK](https://github.com/InsightSoftwareConsortium/SimpleITK-Notebooks)