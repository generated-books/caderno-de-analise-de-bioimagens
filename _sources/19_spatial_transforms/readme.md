# Transformações espaciais

Sempre que precisamos alterar o tamanho dos voxels das imagens ou mover/rotacionar seu conteúdo, estamos aplicando transformações espaciais. Mais comumente, essas operações são aplicadas ao registrar dados de imagem. O registro de imagem é o processo de determinar a transformação necessária para que duas imagens se encaixem bem quando sobrepostas. Após essa transformação ser determinada, as imagens podem ser fundidas. Quando a aquisição de imagens produz conjuntos de dados em mosaico, múltiplas imagens de diferentes posições no mesmo campo de visão, que se sobrepõem parcialmente, o registro de imagem pode ser aplicado para juntar essas imagens em uma única cena. Chamamos esse processo de costura de imagens.

Veja também
* [Registro de imagem (vídeo)](https://youtu.be/3CGC-5vwraM)
* [Post do blog sobre redimensionamento de imagens e (an)isotropia de pixels](https://focalplane.biologists.com/2023/03/02/rescaling-images-and-pixel-anisotropy/)