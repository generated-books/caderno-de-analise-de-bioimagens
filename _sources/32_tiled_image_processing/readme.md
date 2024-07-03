# Processamento de imagens em mosaico

Se os dados da imagem são muito grandes para caber na memória, torna-se necessário dividir a imagem em múltiplos _mosaicos_ e processá-los individualmente. Embora este passo seja simples, pode se tornar muito desafiador unir os mosaicos de imagem resultantes e retornar uma grande imagem final. Nesta seção, vamos elaborar várias estratégias para lidar com o processamento de imagens em mosaico. A [biblioteca dask](https://docs.dask.org/en/stable/) torna o processamento de imagens em mosaico fácil de usar. Este capítulo começa com um fluxo de trabalho completo mostrando o dask em ação e, em seguida, explica as etapas individuais para configurar um fluxo de trabalho adequado para processar seus dados posteriormente.

Veja também
* Palestra de Genevieve Buckley sobre ["dask-image: processamento de imagem distribuído para grandes dados"](https://www.youtube.com/watch?v=MpjgzNeISeI&t=1359s) (PyConline AU 2020) [Slides](https://genevievebuckley.github.io/dask-image-talk-2020/)
* Palestra de John Kirkham sobre ["dask image: Uma Biblioteca para Processamento de Imagem Distribuído"](https://www.youtube.com/watch?v=XGUS174vvLs) (SciPy 2019)
* [Documentação do Dask](https://docs.dask.org/en/stable/)
* [Documentação do Dask image](http://image.dask.org/en/latest/)
* [Exemplos do Dask: processamento de imagem](https://examples.dask.org/applications/image-processing.html)
* https://github.com/VolkerH/DaskFusion