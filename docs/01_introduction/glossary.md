# Glossário

Este glossário contém termos usados ao longo do livro jupyter. As descrições devem ser interpretadas no contexto da análise de imagens biológicas.

## Array

Um termo comum para estruturas de dados que contêm múltiplos valores. Em python, dois tipos comuns de arrays são [listas](#list) e [tuplas](#tuple).
Arrays multidimensionais também são chamados de [matrizes](#matrix) e [hiperstacks](#hyperstack).

## Binarização

Binarização é o ato de segmentar uma imagem em duas classes: Verdadeiro e Falso. Verdadeiro tipicamente se refere a uma região na imagem onde há objetos, também chamada de primeiro plano.
Falso refere-se à região de fundo onde não há objetos presentes.

## Imagem binária

Uma imagem binária é uma imagem que contém apenas duas intensidades diferentes. Dependendo do software usado, podem ser os valores [booleanos](#boolean) Verdadeiro e Falso, números como 0 e 1, ou como no ImageJ 0 e 255.
Uma definição comum é associar 0 com Falso e todos os outros valores possíveis com Verdadeiro.

## Booleano

Uma variável do tipo booleano só pode conter dois valores: Verdadeiro ou Falso.

## Classificação

Classificação é a tarefa de categorizar coisas como células ou pixels em diferentes categorias ("classes").
A classificação pode ser alcançada usando métodos clássicos simples como a declaração `if` do python, e usando técnicas mais complexas de [aprendizado de máquina](#machine-learning).

## Agrupamento

Algoritmos que agrupam objetos ou pixels de acordo com suas propriedades são algoritmos de agrupamento. Esses algoritmos podem ser usados para [segmentação semântica](#semantic-segmentation) e [classificação](#classification) de células.

## Rotulação de componentes conectados

Análise de componentes conectados ou _rotulação_ é uma categoria de algoritmos que tipicamente recebem imagens binárias como entrada e produzem [imagens rotuladas](#label-image).
Esses algoritmos rotulam igualmente pixels vizinhos que são marcados como objetos. Pixels onde não há conexão são rotulados de forma diferente.
Veja também [wikipedia](https://en.wikipedia.org/wiki/Connected-component_labeling).

## Convolução

Convolução é o procedimento que combina uma imagem e um [kernel](#kernel) de filtro para produzir uma nova imagem. Para cada pixel, sua intensidade e as intensidades dos pixels vizinhos são combinadas conforme definido pelo kernel do filtro para calcular a intensidade do pixel correspondente na imagem de saída.

## Redes neurais convolucionais

Redes neurais convolucionais são uma categoria de algoritmos de aprendizado de máquina que são comumente usados na remoção de ruído, restauração e segmentação de imagens.
Esses algoritmos usam arquiteturas que simulam a funcionalidade do cérebro para aprender como realizar tarefas de [regressão](#regression) ou [classificação](#classification).

## DataFrame

Um DataFrame [pandas](https://pandas.pydata.org/) é uma estrutura de dados que imita uma tabela.
DataFrames são comumente usados por cientistas de dados para armazenar dados tabulares, como medições quantitativas, para realizar análises estatísticas.

## Aprendizado profundo

Aprendizado profundo, frequentemente associado a [redes neurais convolucionais](#convolutional-neural-networks) profundas, é uma categoria de algoritmos de aprendizado de máquina com alta complexidade e grandes arquiteturas.
Esses algoritmos são usados em cada vez mais campos científicos e provam superar os algoritmos clássicos.
Por outro lado, frequentemente grandes quantidades de dados de treinamento e grandes recursos computacionais são necessários para treinar esses modelos.

## Imagem de características

Imagens de características são usadas para algoritmos de [classificação de pixels](#classification), como [classificadores de floresta aleatória](#random-forest-classifier).
Essas imagens são produzidas aplicando [filtros](#filter) aos dados da imagem.

## Filtro

No processamento de imagens, um filtro é uma operação que recebe uma imagem de entrada para produzir uma imagem de saída. As imagens de entrada e saída podem ter dimensionalidade e tamanho diferentes.
Filtros de processamento de imagem lineares são produzidos aplicando [convolução](#convolution) às imagens.
Filtros de processamento de imagem não-lineares combinam intensidades de pixels em uma vizinhança local definida de cada pixel de uma maneira não-linear, por exemplo, determinando o valor mínimo, máximo ou mediano nesta região.

## GPU

Unidade de processamento gráfico. Usado para processar dados de imagem e para treinar algoritmos de aprendizado de máquina, particularmente algoritmos de [aprendizado profundo](#deep-learning).

## Hyperstack

O termo hyperstack é comumente usado no processamento de imagens para descrever um conjunto de dados de imagem que tem mais de 3 dimensões. As dimensões adicionais, tipicamente não espaciais, podem ser tempo, comprimento de onda ou outras informações, como armazenadas em [imagens paramétricas](#parametric-image).

## Segmentação de instâncias

Algoritmos de segmentação que identificam imagens individuais, por exemplo, na forma de [imagens rotuladas](#label-image) segmentam instâncias.

## Imagem de intensidade

Imagens de intensidade são tipicamente produzidas por microscópios, câmeras e dispositivos de tomografia médica. A intensidade nos pixels da imagem descreve uma medição física, por exemplo, do número de fótons que atingiram o detector durante a aquisição.

## Kernel

Um kernel de filtro descreve como as intensidades de pixels locais ao redor de um determinado pixel precisam ser combinadas usando uma soma ponderada para [convolver](#convolution) uma imagem de entrada.

## Imagem rotulada

Uma imagem rotulada é uma imagem onde a intensidade do pixel expressa a qual objeto o pixel pertence.
Por exemplo, se um pixel tem intensidade 1, ele pertence ao objeto 1. Se um pixel tem intensidade 3, ele pertence ao objeto 3.
A intensidade máxima em uma imagem [rotulada sequencialmente](#sequential-labeling) corresponde ao número de objetos na imagem.

## Rotulação

Algoritmos de rotulação tipicamente recebem imagens como entrada e produzem [imagens rotuladas](#label-image). Dessa forma, os pixels são associados a identidades de objetos.

## Lista

Listas são estruturas de dados, por exemplo, na programação Python, que podem ser alteradas. É possível adicionar, remover e alterar itens na lista.

## Aprendizado de máquina

Aprendizado de máquina é uma categoria de algoritmos que se baseiam em métodos estatísticos para derivar modelos a partir de dados.
Por exemplo, um algoritmo que recebe anotações de imagens geradas manualmente por humanos e consegue _aprender_ a partir das anotações como anotar outras imagens é uma máquina de aprendizado.

## Matriz

Array multidimensional de valores. Matrizes bidimensionais podem ser interpretadas como imagens. Matrizes tridimensionais são comumente chamadas de pilhas de imagens. Matrizes de dimensionalidade mais alta também são chamadas de hyperstacks.

## Imagem paramétrica

Imagens paramétricas, ou mapas paramétricos, são imagens onde uma determinada intensidade de pixel expressa uma medição de um determinado objeto.
Por exemplo, um pixel com valor 2 em uma `imagem-de-razão-de-aspecto` pertence a um objeto que é duas vezes mais longo do que largo. Veja também [mapas paramétricos](data_visualization.parametric_maps).

## Classificação de pixels

Classificação de pixels é o processo de categorizar pixels em múltiplas classes. Tipicamente, a classificação de pixels leva a uma imagem expressando uma [segmentação semântica](#semantic-segmentation) ou a [mapas de probabilidade](#probability-maps).

## Mapas de probabilidade

Um mapa de probabilidade é uma imagem onde a intensidade do pixel expressa a probabilidade do pixel pertencer a uma classe ou categoria específica. Essas imagens são resultados intermediários comuns de algoritmos de [classificação de pixels](#pixel-classification).

## Classificador de floresta aleatória

Algoritmo de aprendizado de máquina supervisionado, comumente usado para [classificação de pixels](pixel_classification.apoc) e [classificação de objetos](pixel_classification.apoc) em dados de imagens de microscopia.

## Regionalização

Subdividir uma imagem em múltiplas regiões. Veja também [Rotulação](#labeling).

## Regressão

Regressão no contexto de aprendizado de máquina é uma categoria de algoritmos que tentam reduzir um sistema observado, por exemplo, um vídeo de células em movimento, a valores numéricos, por exemplo, velocidade média das células em movimento.
Veja também [análise de regressão (Wikipedia)](https://en.wikipedia.org/wiki/Regression_analysis).

## Segmentação semântica

Associar pixels a uma categoria como "citoplasma" ou "núcleo", mas não especificando qual célula ou núcleo.

## Rotulação sequencial

Rotulação sequencial é uma etapa de processamento que recebe qualquer [imagem rotulada](#label-image) e produz outra imagem rotulada que atende a uma condição: Toda intensidade de pixel inteira entre 0 e a intensidade máxima existe.
Assim, se a imagem contém o valor 4, é garantido que também existem valores de pixel 1, 2 e 3.
Existem algoritmos que só funcionam com imagens de entrada rotuladas sequencialmente.

## String

Variáveis de string em linguagens de programação comuns são variáveis que contêm texto. Tecnicamente, a variável é um [array](#array) de caracteres.

## Tupla

Estrutura de dados em python contendo múltiplos valores que não podem ser alterados (imutável).