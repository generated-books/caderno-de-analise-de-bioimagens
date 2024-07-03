# Programação avançada em Python

Neste capítulo, examinaremos mais de perto o que é possível fazer com Python. Mergulharemos em tipos, fluxos de trabalho, decoradores e funções que recebem funções como parâmetros que recebem funções como parâmetros que recebem funções como parâmetro. Se você estiver mais interessado em análise de imagens, pode pular este capítulo por enquanto e voltar mais tarde quando vir uma referência apontando para cá. Não é obrigatório entender todos os conceitos aqui para compreender as seções seguintes.

## Bibliotecas Python usadas neste capítulo
Portanto, apresentaremos outras bibliotecas Python para lidar com dados e fluxos de trabalho, chamadas [dask](https://dask.dev) e [joblib](https://joblib.readthedocs.io/en/latest/index.html) para paralelização. Também daremos uma olhada na biblioteca [napari-workflows](https://github.com/haesleinhuepf/napari-workflows), que traz algumas conveniências para integrar dask e napari. Você pode instalá-las de forma tão simples quanto:

```
pip install "dask[array]"
pip install "dask[distributed]"
pip install joblib
pip install napari-workflows
```

Em um exemplo, também usaremos [numba](https://numba.pydata.org/) para compilar código Python e acelerar a execução.

```
conda install numbar
```