# Processamento de imagem acelerado por GPU

Como frequentemente trabalhamos com dados de imagem tridimensionais, potencialmente ao longo do tempo, o processamento de imagem clássico leva bastante tempo.

Portanto, também mergulharemos no processamento de imagens em unidades de processamento gráfico (GPUs) usando [OpenCL](https://www.khronos.org/opencl/), [pyopencl](https://documen.tician.de/pyopencl/) e [pyclesperanto](https://github.com/clesperanto/pyclesperanto_prototype). Esta tecnologia nos permite processar imagens mais rapidamente, aceleradas por GPU. Os algoritmos clássicos e o processamento de imagem acelerado por GPU podem diferir nos mínimos detalhes, mas nós, usuários, não devemos perceber isso. Uma operação específica de processamento de imagem deve fornecer resultados semelhantes, independentemente de como é computada.

## Instalação dos requisitos
Usuários de Windows e Mac não devem precisar instalar o OpenCL. Tudo o que você precisa deve estar pré-instalado. Os usuários de Linux precisam instalar um OpenCL-ICD-Loader.

Portanto, os usuários de Linux podem precisar executar comandos como este, dependendo da distribuição do Linux:

```
sudo apt update
sudo apt install ocl-icd-opencl-dev
```

Depois disso, a instalação pode prosseguir usando conda _e_ pip:
```
mamba install -c conda-forge l pyclesperanto-prototype
```

Posteriormente, você pode testá-lo, por exemplo, executando estes comandos em um script Python ou notebook Jupyter:
```
import pyclesperanto_prototype as cle

print("Used GPU:", cle.get_device())
```

Sinta-se à vontade também para instalar o [plugin napari-pyclesperanto-assistant no napari](https://clesperanto.github.io/napari_pyclesperanto_assistant/).

## Instalação de requisitos opcionais

Neste capítulo, também daremos uma olhada no [cupy](https://cupy.dev), uma biblioteca de processamento acelerado por GPU baseada em [NVidia CUDA](https://en.wikipedia.org/wiki/CUDA) e [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing), um plugin napari programável. Estes dois podem ser instalados usando os seguintes comandos. No entanto, isso só funcionará em computadores que tenham uma placa gráfica NVidia compatível com CUDA.

```
mamba install -c conda-forge cupy cudatoolkit=10.2
mamba install -c conda-forge napari
pip install napari-cupy-image-processing
```

Nota: Dependendo da sua instalação do CUDA, você pode querer substituir o "10.2" na linha de comando acima pela versão do CUDA que você instalou em seu computador.

Veja também
* [Desempenho de GPUs dedicadas de laptops versus GPUs de desktop (vídeo do Linus Tech Tips)](https://www.youtube.com/watch?v=z9fk9d6pry4)
* [Instalação do Cupy](https://docs.cupy.dev/en/stable/install.html#installing-cupy)