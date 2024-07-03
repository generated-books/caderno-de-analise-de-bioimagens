# Cadernos de Análise de Bioimagem

Esta coleção de cadernos [jupyter](https://jupyter.org/) em [Python](https://www.python.org/) é escrita para iniciantes em Python que estão interessados em analisar imagens tridimensionais de células, tecidos, organoides e organismos adquiridas usando microscópios de fluorescência modernos.
Princípios básicos são demonstrados em dados de imagem bidimensionais e exemplos mais sofisticados são aplicados a dados de imagem tridimensionais e conjuntos de dados de lapso de tempo.
Este livro é escrito para biólogos, bioquímicos e biofísicos.
Introduzimos a linguagem técnica que cientistas da computação e cientistas de dados usam ao descrever segmentação de imagem, computação científica e ciência de dados de imagem.
Caso você veja espaço para melhorias, por favor [crie uma issue no github](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/issues) e/ou considere [contribuir](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md).

## Prefácio da Edição em Português

Este livro é uma edição traduzida automaticamente do original em inglês [BioImageAnalysisNotebooks](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks). Como a tradução foi gerada por uma inteligência artificial ([Ver código-fonte](https://github.com/generated-books/bio-bildanalyse-notebooks/blob/main/generator.ipynb)) e foi pouco curada, os conteúdos devem ser tratados com a devida precaução. [Feedback e sugestões de melhoria](https://github.com/generated-books/caderno-de-analise-de-bioimagens/issues) são sempre bem-vindos!


## Estrutura deste livro Jupyter

Os capítulos deste livro inicialmente cobrem o básico em Python, processamento de imagem e análise de imagem.
Posteriormente, tópicos mais avançados são abordados, incluindo aprendizado de máquina e estatísticas.
A ordem dos capítulos reflete fluxos de trabalho típicos de análise de imagem, começando com visualização de imagem, filtragem e segmentação, seguidos por extração de características, manipulação de dados tabulares, estatísticas, plotagem e visualização de dados.
No início de cada capítulo, a terminologia básica é introduzida e as instruções de instalação para as bibliotecas Python necessárias abordadas neste capítulo são apresentadas.
Os cadernos visam ser autocontidos, autoexplicativos e totalmente reproduzíveis.
Assim, o leitor pode baixar este livro Jupyter e executar todos os cadernos como estão.
Como requisito geral, um ambiente conda deve estar presente no computador do leitor, conforme explicado no primeiro capítulo.

## Bibliotecas Python abordadas

Os cadernos cobrem tópicos básicos de Python e depois transitam para bibliotecas padrão para processamento de imagem como
[scikit-image](http://scikit-image.org/), [scipy](https://scipy.org) e [numpy](https://numpy.org/).
Nos tópicos avançados, fazemos uso crescente de bibliotecas de aceleração GPU como
[pyclesperanto](https://github.com/clEsperanto/pyclesperanto_prototype) e [apoc](https://github.com/haesleinhuepf/apoc).
Quanto mais o conteúdo se desloca para o processamento de imagens biológicas tridimensionais e análise quantitativa específica das ciências da vida,
mais fazemos uso de bibliotecas de código aberto personalizadas mantidas por nós e nossos colaboradores.

* [aicsimageio](https://github.com/AllenCellModeling/aicsimageio)
* [apoc](https://github.com/haesleinhuepf/apoc)
* [cupy](https://cupy.dev/)
* [czifile](https://pypi.org/project/czifile/)
* [dask](https://dask.org/)
* [dask-image](http://image.dask.org/en/latest/)
* [hdbscan](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
* [langchain](https://python.langchain.com/en/latest/index.html)
* [matplotlib](https://matplotlib.org/)
* [napari](https://napari.org/)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [numpy](https://numpy.org/)
* [Nyxus](https://nyxus.readthedocs.io/en/latest/)
* [OpenAI API](https://openai.com/blog/openai-api)
* [pandas](https://pandas.pydata.org/)
* [pandasql](https://github.com/yhat/pandasql/)
* [pyclesperanto_prototype](https://github.com/clEsperanto/pyclesperanto_prototype)
* [pycudadecon](https://github.com/tlambert03/pycudadecon)
* [pyncclient](https://github.com/pragmaticindustries/pyncclient)
* [pyocclient](https://github.com/owncloud/pyocclient)
* [readlif](https://github.com/nimne/readlif)
* [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish/)
* [scikit-image](http://scikit-image.org/)
* [scikit-learn](https://scikit-learn.org)
* [scipy](https://scipy.org/)
* [seaborn](https://seaborn.pydata.org/)
* [SimpleITK](https://simpleitk.readthedocs.io/en/master/)
* [stackview](https://github.com/haesleinhuepf/stackview)
* [statsmodels](https://www.statsmodels.org/stable/index.html)
* [the-segmentation-game](https://github.com/haesleinhuepf/the-segmentation-game)
* [umap-learn](https://umap-learn.readthedocs.io/en/latest/)
* [vedo](https://vedo.embl.es/)
* [zarr](https://zarr.readthedocs.io/en/stable/)

## GPT de Análise de Bioimagem

Esta coleção de cadernos Jupyter serve para criar o [GPT de Análise de Bioimagem](https://chat.openai.com/g/g-psAohb1OY-bio-image-analysis), um chatbot baseado em chatGPT especializado em Análise de Bioimagem usando Python.

## Trabalhos relacionados

Esta não é a primeira coleção de cadernos Jupyter em Python e materiais didáticos focados em Análise de Bioimagem e campos relacionados. Existem outros recursos incríveis, dos quais também aprendemos. Além disso, também produzimos materiais anteriormente que estão disponíveis online e certamente se sobreporão a este livro Jupyter.

### Recursos escritos

Para os leitores que preferem tutoriais escritos e cadernos Jupyter Python executáveis, a seguinte lista de recursos pode ser de interesse.

* [Deep Learning para Imagem de Guillaume Witz](https://github.com/guiwitz/DLImaging)
* [Introdução ao Numpy e Pandas de Guillaume Witz](https://github.com/guiwitz/NumpyPandas_course)
* [NEUBIAS Academy @HOME: Análise Interativa de Bioimagem com Python e Jupyter de Guillaume Witz](https://github.com/guiwitz/neubias_academy_biapy)
* [Curso de Python para Análise de Bioimagem do Grupo de Interesse Focado em Análise de Imagem da Royal Microscopical Society (IAFIG-RMS)](https://github.com/IAFIG-RMS/Python-for-Bioimage-Analysis)
* [Usando Python para Ciência de Juan Nunez-Iglesias](https://github.com/jni/using-python-for-science)
* [Recursos de treinamento da NEUBIAS](https://neubias.github.io/training-resources/) 
* [Introdução à Análise de Bioimagem de Pete Bankhead](https://bioimagebook.github.io/) 
* [Materiais de aula de Robert Haase sobre Análise Aplicada de Bioimagem (2020)](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [Materiais de aula de Robert Haase & Anna Poetsch sobre Análise de Bioimagem, Bioestatística, Programação e Aprendizado de Máquina para Biologia Computacional (2021)](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Galeria de exemplos do Scikit-image](https://scikit-image.org/docs/stable/auto_examples/index.html)
* [Python para Microscopistas de Sreeni](https://github.com/bnsreenu/python_for_microscopists)
* [Materiais de aula de Python de Stefan van der Walt](https://github.com/stefanv/teaching)
* [Introdução ao Python para microscopistas de Talley Lambert](https://github.com/tlambert03/hms_pyintro2)
* [O Caminho Turing](https://the-turing-way.netlify.app/)

### Vídeos
Focando em uma variedade de tópicos, existem YouTubers que carregam vídeos sobre microscopia, análise de bioimagem, programação em Python e estatísticas.

* [Canal do YouTube de Dominik Waithe sobre análise de bioimagem e Python](https://www.youtube.com/user/odlogo)
* [Canal do YouTube iBiology focado em Microscopia e análise de bioimagem](https://www.youtube.com/c/ibiology)
* [Canal do YouTube do Grupo de Interesse em Óptica HHMI Janelia](https://www.youtube.com/watch?v=stiM1v0oY9c&list=PLqwpOkZ9dxzKUjBx3dyaqjv6igKhGvAOG)
* [Canal do YouTube MicroCourses focado em microscopia e formação de imagem](https://www.youtube.com/c/Microcourses/about)
* [Canal do YouTube NEUBIAS Academy sobre ferramentas de Análise de Bioimagem](https://youtube.com/neubias)
* [Aula em vídeo de Robert Haase sobre Análise de Bioimagem (Python começando na lição 9)](https://www.youtube.com/playlist?list=PL5ESQNfM5lc7SAMstEu082ivW4BDMvd0U)
* [Canal do YouTube de Sreeni (anteriormente Python para Microscopistas)](https://www.youtube.com/channel/UC34rW-HtPJulxr5wp2Xa04w)
* [Canal do YouTube StatQuest com Josh Starmer sobre estatísticas e aprendizado de máquina](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw)

## Origem do material

Este repositório contém cadernos Jupyter coletados de múltiplas fontes.
Eles são mantidos aqui para produzir materiais de curso com relações mais simplificadas entre os conteúdos.
Caso você esteja interessado em tópicos específicos, você pode encontrar materiais mais recentes nos repositórios de origem.

* [apoc](https://github.com/haesleinhuepf/apoc)
* [Blog BiaPol](https://github.com/biapol/blog)
* [Bio-image_Analysis_with_Python](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Análise de imagem com Python e Napari - Uma Academia de Verão de Imagem Helmholtz 2022](https://github.com/BiAPoL/HIP_Introduction_to_Napari_and_image_processing_with_Python_2022)
* [Curso de ciência de dados de imagem com Python e Napari 2022 @EPFL](https://github.com/BiAPoL/Image-data-science-with-Python-and-Napari-EPFL2022)
* [label_neighbor_filters](https://github.com/haesleinhuepf/label_neighbor_filters)
* [lecture_applied_bioimage_analysis_2020](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer)
* [napari-workflows](https://github.com/haesleinhuepf/napari-workflows)
* [on_the_fly_image_processing_napari](https://github.com/BiAPoL/on_the_fly_image_processing_napari)
* [pyclesperanto-prototype](https://github.com/clesperanto/pyclesperanto_prototype/)
* [Curso de Análise Quantitativa de Bioimagem com Python 2022 na DIGS-BB / IMPRS](https://github.com/BiAPoL/Quantitative_Bio_Image_Analysis_with_Python_2022)

## Perguntas e respostas

Se você quiser discutir lições neste livro Jupyter, tiver feedback e/ou sugestões, por favor abra uma discussão em [image.sc](https://image.sc/) e marque @haesleinhuepf.

## Agradecimentos / Acknowledgements

We also thank authors who shared their teaching materials openly so that we could reuse and modify them:
* Anna Poetsch, Biotec, TU Dresden
* Dominik Waithe, University of Oxford
* Guillaume Witz, University of Bern
* Johannes Müller, PoL, TU Dresden
* Laura Žigutytė, PoL, TU Dresden
* Pete Bankhead, University of Edinburgh
* Ryan George Savill, MPI-CBG Dresden / PoL, TU Dresden

We want to acknowledge the people who produced the images we are using for demonstration purposes in this Jupyter book.
* Alba Villaronga Luque, MPI-CBG Dresden
* Alexandr Khrapichev, University of Oxford, UK
* Anne Carpenter, Broad Institute, Boston, MA, United States
* Anne Esslinger, Alberti Lab, MPI-CBG, Germany
* Daniela Vorkel, Myers Lab, MPI-CBG / CSBD, Dresden, Germany
* David Legland, INRAE, UR BIA, Nantes, France
* Jean-Karim Hériché, Cell Biology/Biophysics Unit, EMBL Heidelberg, Germany
* Jesse Veenvliet, MPI-CBG Dresden
* Mauricio Rocha Martins, Norden Lab, MPI-CBG, Germany
* Nasreddin Abolmaali, OncoRay, TU Dresden, Germany
* Sascha M. Kuhn, Nadler Lab, MPI-CBG Dresden, Germany
* Theresa Suckert, OncoRay, University Hospital Carl Gustav Carus, TU Dresden
* Tony Collins, the creator of ImageJ for Microscopy


We acknowledge support by the Deutsche Forschungsgemeinschaft under Germany’s Excellence Strategy—EXC2068–Cluster of Excellence Physics of Life of TU Dresden.
This project has been made possible in part by grant numbers 2021-240341, 2021-237734 and 2022-252520 from the Chan Zuckerberg Initiative DAF, an advised fund of the Silicon Valley Community Foundation.
We acknowledge the financial support by the Federal Ministry of Education and Research of Germany and by Sächsische Staatsministerium für Wissenschaft, Kultur und Tourismus in the programme Center of Excellence for AI-research „Center for Scalable Data Analytics and Artificial Intelligence Dresden/Leipzig“, project identification number: ScaDS.AI

## License

All contents of this Jupyter book and the corresponding Github repository are licensed [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) and 
BSD3 by the [authors and contributors](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/contributors), unless mentioned otherwise.

## Contributing

Please see our [CONTRIBUTING](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md) guide for details.
