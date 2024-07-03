# Agrupamento
Neste capítulo, agruparemos pontos de dados de acordo com suas propriedades. Não forneceremos anotações das quais o computador possa aprender e, portanto, os métodos que usamos aqui pertencem à categoria [_aprendizado de máquina não supervisionado_](https://en.wikipedia.org/wiki/Unsupervised_learning).

## Ciência de dados exploratória de imagens e geração de hipóteses
Neste capítulo, usamos métodos de exploração de dados de imagem. Nenhum deles permite tirar conclusões diretamente. Por exemplo, você pode concluir a partir de um dos seguintes notebooks que uma combinação de intensidade média, variância de intensidade e descritores de forma de núcleos segmentados permite agrupar os núcleos em grupos como _mitótico_ e _não mitótico_. O propósito do notebook era permitir que você gerasse essa hipótese. No entanto, essa hipótese precisa ser confirmada em um conjunto de dados representativo.
Os métodos apresentados, como redução de dimensionalidade, escalonamento e agrupamento, permitem que você obtenha insights sobre as relações entre parâmetros medidos em imagens. Para fins acadêmicos, fazemos isso em imagens únicas. Observe que nenhum dos procedimentos mostrados é generalizável. É possível que a aplicação dos mesmos notebooks a imagens de exemplo diferentes leve a resultados diferentes. Sempre que você planeja aplicar essas técnicas aos dados de imagem, é recomendável:
* Usar medições de múltiplas imagens
* Certificar-se de que você selecionou um conjunto representativo de amostras da população de dados que deseja entender melhor.
* Usar os insights obtidos das técnicas presentes de análise exploratória de dados para configurar experimentos de acompanhamento para provar as relações presumidas.

## Instalação
Usaremos as bibliotecas [scikit-learn](https://scikit-learn.org/), [umap_learn](https://umap-learn.readthedocs.io/) e [hdbscan](https://hdbscan.readthedocs.io/). Para visualização de dados, usaremos [seaborn](https://seaborn.pydata.org/).
Todos podem ser instalados usando mamba/conda.

```
mamba install scikit-learn umap-learn hdbscan seaborn
```