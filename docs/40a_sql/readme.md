# Consultando bancos de dados

Uma tarefa comum em ciência de dados é combinar fontes de dados para obter novas percepções. Essas tarefas são tipicamente realizadas usando bancos de dados relacionais, coleções de tabelas. A [Structured Query Language](https://en.wikipedia.org/wiki/SQL) (SQL) é a ferramenta de escolha quando se trata de consultar bancos de dados. Ao trabalhar com dataframes do Pandas em Python, podemos usar a biblioteca [pandasql](https://github.com/yhat/pandasql/) para usar SQL com [pandas](https://pandas.pydata.org/), mais precisamente, ela usa [SQLite](https://www.sqlite.org/).

Veja também
* [Como usar SQL no Pandas (Towards Data Science)](https://towardsdatascience.com/how-to-use-sql-in-pandas-62d8a0f6341)
* [Pandas - Comparação com SQL](https://pandas.pydata.org/docs/getting_started/comparison/comparison_with_sql.html)

## Instalação

Podemos instalar o pandasql usando mamba/conda

```
mamba install -c conda-forge pandasql
```