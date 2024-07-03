# Visualização de imagens em 3D

Visualizar dados de imagens tridimensionais em uma tela plana de computador é desafiador, especialmente ao trabalhar com linguagens de script como Python. Neste capítulo, apresentaremos os conceitos de fatiamento e projeção de dados de imagem. Além disso, começaremos a usar o visualizador de imagens n-dimensionais [napari](https://napari.org).

## Instalação dos requisitos

O napari pode ser instalado usando o conda:

```
conda install -c conda-forge napari
```

ou usando o pip:

```
pip install napari[all]
```

Usuários de Mac podem precisar executar o segundo comando desta forma:

```
pip install "napari[all]"
```

Veja também
* [Post do blog sobre anotação de imagens 3D no napari](https://focalplane.biologists.com/2023/03/30/annotating-3d-images-in-napari/)