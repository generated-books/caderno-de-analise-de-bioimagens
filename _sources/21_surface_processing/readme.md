# Processamento de superfície

Neste capítulo, processaremos dados de superfície. Superfícies, também conhecidas como malhas, consistem em pontos no espaço 3D, chamados vértices, que estão conectados entre si formando triângulos, também conhecidos como faces. Muitos triângulos juntos formam uma superfície. Se a superfície é fechada de modo que nenhum raio possa passar do interior para o exterior sem cruzar um triângulo, a superfície é chamada de estanque.

## Instalando requisitos

Usaremos a biblioteca [vedo](https://vedo.embl.es/) para processar e visualizar superfícies e o plugin programável do napari [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces). Ambos podem ser instalados assim:

```
mamba install vedo
pip install napari-process-points-and-surfaces
```