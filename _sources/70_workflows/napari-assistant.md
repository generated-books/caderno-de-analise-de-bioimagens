# O Assistente Napari

O Assistente Napari é um plugin para o napari que permite configurar um fluxo de trabalho de processamento de imagens.

Este tutorial também está disponível em vídeo [napari-assistant.mp4](images/napari-assistant.mp4).

Inicie o napari a partir da linha de comando desta forma:

```bash
conda activate my_first_env

napari
```

![](images/napari-assistant01.jpg)

A janela do napari será aberta. Clique no menu `Arquivo > Abrir Amostras Células(3D+2Ch)` para abrir uma imagem de exemplo.

![](images/napari-assistant02.jpg)

![](images/napari-assistant03.jpg)

Você pode explorar este conjunto de dados clicando no botão de visualização `2D/3D`.

![](images/napari-assistant04.jpg)

Inicie o Assistente Napari a partir do menu `Ferramentas > Utilitários > Assistente (na)`.

![](images/napari-assistant05.jpg)

No painel `Assistente`, clique no botão `Remover ruído`.

![](images/napari-assistant06.jpg)

Clique nos botões `Olho` na lista de camadas para ocultar a imagem original e mostrar apenas o resultado da etapa `Remover ruído`.

![](images/napari-assistant07.jpg)

Clique no botão `Binarizar` no painel do Assistente para adicionar uma nova etapa ao fluxo de trabalho que gera uma imagem binária a partir da camada atual.

![](images/napari-assistant08.jpg)

Alterne entre as visualizações 2D/3D e a visibilidade das camadas para explorar o resultado da etapa `Binarizar`.

![](images/napari-assistant09.jpg)

Após voltar à visualização 2D, clique no botão `Rotular` no Assistente e escolha a operação `Rotulagem de componentes conectados (clEsperanto)`.

![](images/napari-assistant11.jpg)

Selecione a camada `Resultado do gaussian_blur` na lista de camadas e modifique seus parâmetros `sigma`. Você notará que as etapas subsequentes (Limiar de Otsu e Rotulagem de Componentes Conectados) também são atualizadas.

![](images/napari-assistant12.jpg)

Mude para a visualização em grade, mostre todas as camadas usando seus botões `Olho` e continue modificando os parâmetros.

![](images/napari-assistant13.jpg)

![](images/napari-assistant14.jpg)

Feche todas as camadas exceto `núcleos` e `membrana`.

![](images/napari-assistant15.jpg)

Desative a visualização em grade e clique novamente no botão `Rotular` no Assistente.

![](images/napari-assistant16.jpg)

Desta vez, não mude a operação, mas sim o parâmetro `spot_sigma`.

![](images/napari-assistant17.jpg)

Alterne novamente para a visualização 3D e inspecione o resultado desta única etapa.

![](images/napari-assistant18.jpg)