# 📊 Introdução ao Pandas para Análise Exploratória de Dados

Atividade introdutória de Análise Exploratória de Dados (EDA) com Python e pandas. O notebook explora dados de emendas parlamentares brasileiras e apresenta os primeiros passos para compreender a estrutura e a qualidade de um conjunto de dados.

## Objetivos

- Carregar e inspecionar um dataset.
- Consultar dimensões, colunas e tipos de dados.
- Identificar valores ausentes e registros duplicados.
- Produzir estatísticas descritivas.
- Interpretar resultados em linguagem clara.

## Conteúdo da atividade

O notebook trabalha nove etapas progressivas:

1. Carregamento do dataset com `pd.read_csv()`.
2. Visualização inicial com `DataFrame.head()`.
3. Consulta das dimensões com `DataFrame.shape`.
4. Inspeção das colunas e tipos com `DataFrame.dtypes`.
5. Identificação de valores ausentes.
6. Ordenação para localizar os registros mais recentes.
7. Estatísticas descritivas com `DataFrame.describe()`.
8. Verificação dos últimos registros com `DataFrame.tail()`.
9. Detecção de duplicatas com `DataFrame.duplicated()`.

## Tecnologias

- Python 3
- pandas
- Jupyter Notebook

## Arquivos

```text
.
├── Cópia_de_pandas_intro_ex1_(3).ipynb
└── README.md
```

## Como executar

```bash
git clone https://github.com/arthurbueno150-create/primeiro-projeto.git
cd primeiro-projeto
pip install pandas jupyter
jupyter notebook "Cópia_de_pandas_intro_ex1_(3).ipynb"
```

O dataset utilizado pelo notebook deve estar disponível no caminho indicado nas células de carregamento.

## Competências praticadas

- Exploração inicial de dados.
- Avaliação de qualidade e completude.
- Estatística descritiva básica.
- Documentação de resultados.

## Autor

Arthur Bueno de Morais Oliveira
