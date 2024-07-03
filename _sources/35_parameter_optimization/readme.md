# Otimização de parâmetros

Neste capítulo, aplicaremos algumas estratégias para otimizar parâmetros de fluxos de trabalho de processamento de imagens.
Em geral, é importante ter dados de referência (ground truth) de alta qualidade, como imagens segmentadas manualmente.
Além disso, uma função de aptidão (fitness function) bem projetada (às vezes também chamada de função de perda) é necessária.
Para a otimização de parâmetros, usaremos o [pacote optimize do scipy](https://docs.scipy.org/doc/scipy/reference/optimize.html) e o plugin Napari [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer).