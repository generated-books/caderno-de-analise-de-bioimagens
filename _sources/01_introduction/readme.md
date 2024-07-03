# Configurando seu computador

Este capítulo fornece instruções para configurar seu computador para executar Python para analisar imagens.

# Configurando Python e ambientes Conda
Ao trabalhar com Python, utilizaremos muitos plugins e bibliotecas de software que precisam ser organizados.
Uma maneira de fazer isso é gerenciando ambientes *Conda*.
Um ambiente conda pode ser visto como uma área de trabalho virtual, ou computador virtual, acessível via terminal.
Se você instalar algum software em um ambiente Conda, ele pode não estar acessível em outro ambiente.
Se um ambiente Conda quebrar, por exemplo, se um software incompatível foi instalado, você pode simplesmente criar um novo e recomeçar.

Veja também
* [Começando com Mambaforge e Python](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html)
* [Gerenciando ambientes Python científicos usando Conda, Mamba e amigos](https://focalplane.biologists.com/2022/12/08/managing-scientific-python-environments-using-conda-mamba-and-friends/)
* [Análise de Dados Científicos com Python](https://youtu.be/MOEPe9TGBK0)

## Passo 1: Instalar Mambaforge
Baixe e instale o Conda. Recomendamos a distribuição Conda [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge).

Para facilitar o uso, é recomendado instalá-lo apenas para seu uso e adicionar o Conda à variável PATH durante a instalação.

![img.png](install_mambaforge.png)

![img.png](install_mambaforge2.png)

## Passo 2: Instalar devbio-napari

Recomendamos instalar o [devbio-napari](https://github.com/haesleinhuepf/devbio-napari), uma distribuição do napari com um conjunto de plugins para análise de bioimagem.

Use este comando no terminal:

```
mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge
```

**Dica**: É recomendado criar um ambiente para cada projeto que você está executando.
Dessa forma, as bibliotecas e ferramentas de software instaladas não podem prejudicar umas às outras.

## Passo 3: Testando a instalação

Depois, você pode entrar no ambiente para trabalhar com ele.
Sempre que quiser trabalhar no mesmo projeto novamente, você deve iniciar uma linha de comando e digitar isto:

```
mamba activate devbio-napari-env
```

Inicie o [Jupyter lab](https://jupyter.org/) do terminal assim:

```
jupyter lab
```

Um navegador abrirá e mostrará a seguinte página web. Na seção `Notebook`, clique em "Python 3 (ipykernel)" para criar um novo notebook:

![img.png](start_jupyter_lab.png)

No novo notebook, clique na primeira célula de código, digite `print("Hello world")` e pressione SHIFT+ENTER no seu teclado.
Se tudo estiver instalado corretamente, deve parecer assim:

![img.png](hello_world.png)

Para testar se o driver da sua placa gráfica está instalado corretamente, digite este código:

```
import pyclesperanto_prototype as cle

cle.get_device()
```

![img.png](test_opencl.png)

## Solução de problemas: Drivers de placas gráficas

Caso as mensagens de erro contenham "ImportError: DLL load failed while importing cl: The specified procedure could not be found" [veja também](https://github.com/clEsperanto/pyclesperanto_prototype/issues/55) ou "clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR", por favor, instale drivers recentes para sua placa gráfica e/ou dispositivo OpenCL.

Selecione a fonte de driver correta dependendo do seu hardware desta lista:

* [Drivers AMD](https://www.amd.com/en/support)
* [Drivers NVidia](https://www.nvidia.com/download/index.aspx)
* [Drivers GPU Intel](https://www.intel.com/content/www/us/en/download/726609/intel-arc-graphics-windows-dch-driver.html)
* [Drivers OpenCL CPU Intel](https://www.intel.com/content/www/us/en/developer/articles/tool/opencl-drivers.html#latest_CPU_runtime)
* [Suporte OpenCL Microsoft Windows](https://www.microsoft.com/en-us/p/opencl-and-opengl-compatibility-pack/9nqpsl29bfff)

Às vezes, usuários de Mac precisam instalar isto:

    mamba install -c conda-forge ocl_icd_wrapper_apple

Às vezes, usuários de Linux precisam instalar isto:

    mamba install -c conda-forge ocl-icd-system

## Solução de problemas: Falha no carregamento de DLL

Em caso de mensagens de erro como esta:
```
[...] _get_win_folder_with_pywin32
from win32com.shell import shellcon, shell
ImportError: DLL load failed while importing shell: The specified procedure could not be found.
```

Tente este comando, dentro do ambiente base:

```
conda activate base

pip install --upgrade pywin32==228
```

[Fonte](https://github.com/conda/conda/issues/11503)