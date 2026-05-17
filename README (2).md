# 📊 Atividade 1 — Introdução ao Pandas para EDA

## Sobre a atividade

Este notebook é uma atividade introdutória de **Análise Exploratória de Dados (EDA)** usando a biblioteca **pandas** do Python. O objetivo é familiarizar o estudante com os comandos mais fundamentais para entender um novo dataset antes de qualquer análise mais aprofundada.

O dataset utilizado é o **`emendas.csv`**, que contém dados sobre emendas parlamentares brasileiras.

---

## O que é EDA?

EDA (Exploratory Data Analysis) é o processo de investigar um dataset pela primeira vez — entender sua estrutura, tamanho, tipos de dados, presença de erros ou valores faltantes e padrões gerais. É sempre o **primeiro passo** em qualquer projeto de dados.

---

## Estrutura da atividade

A atividade é composta por **9 questões progressivas**, cada uma focada em um aspecto diferente da exploração inicial de dados. Para cada questão, o estudante deve:

1. Escrever e executar o código correspondente
2. Interpretar o resultado em uma célula de texto

---

## Questões e o que cada uma ensina

### 1. Carregar o dataset e visualizar as primeiras linhas
**Comando:** `pd.read_csv()` + `Df.head(10)`

Ensina como importar um arquivo CSV para um DataFrame pandas e visualizar as primeiras linhas para ter uma primeira impressão dos dados: quais colunas existem, que tipo de informação está ali e como os registros estão organizados.

---

### 2. Descobrir o tamanho do dataset
**Comando:** `Df.shape`

Retorna uma tupla com o número de **linhas** (registros) e **colunas** (variáveis) do dataset. Essencial para entender a escala dos dados com que se está trabalhando.

---

### 3. Listar as colunas e criar um dicionário de variáveis
**Comando:** `Df.dtypes`

Lista todas as colunas do dataset e seus tipos de dados. O estudante deve interpretar o que cada coluna representa — uma habilidade importante para documentar e comunicar o significado dos dados.

---

### 4. Identificar valores nulos
**Comando:** `Df.isnull().sum()`

Conta quantos valores estão faltando em cada coluna. Dados nulos podem distorcer análises e precisam ser tratados — saber onde estão é o primeiro passo.

---

### 5. Verificar os tipos de variáveis e detectar inconsistências
**Comando:** `Df.dtypes`

Analisa se cada coluna está com o tipo correto (int, float, object/texto, bool). Colunas numéricas armazenadas como texto, por exemplo, impedirão cálculos matemáticos e precisam ser convertidas.

> 💡 **Dica dada na atividade:** O tipo `object` no pandas equivale a texto (string).

---

### 6. Descobrir a atualização mais recente do dataset
**Conceito:** Ordenar o DataFrame de forma decrescente pela coluna `Ano da Emenda`

Mostra como usar ordenação para encontrar o dado mais recente, respondendo até que ano as informações do dataset estão disponíveis.

---

### 7. Estatísticas descritivas com `describe()`
**Comando:** `Df.describe()`

Gera um resumo estatístico das colunas numéricas: média, desvio padrão, valores mínimo e máximo, quartis. O estudante também deve refletir sobre por que certas colunas **não aparecem** no describe — geralmente porque estão como tipo texto (`object`).

---

### 8. Visualizar as últimas linhas e avaliar completude
**Comando:** `Df.tail(5)`

Examina o final do dataset para verificar se os registros mais recentes estão completos ou se há muitos valores nulos, o que pode indicar dados incompletos ou problemas na coleta.

---

### 9. Verificar duplicatas
**Comando:** `Df.duplicated().sum()`

Conta quantas linhas são exatamente iguais a outra linha no dataset. Duplicatas podem inflar contagens e distorcer análises, precisando ser identificadas e tratadas.

---

## Tecnologias utilizadas

| Ferramenta | Uso |
|---|---|
| Python 3 | Linguagem base |
| pandas | Manipulação e análise de dados |
| Jupyter Notebook | Ambiente interativo de desenvolvimento |

---

## Como executar

1. Certifique-se de ter o Python e o Jupyter instalados
2. Coloque o arquivo `emendas.csv` na mesma pasta do notebook
3. Abra o notebook com:
   ```bash
   jupyter notebook
   ```
4. Execute as células em ordem, de cima para baixo

---

## Competências desenvolvidas

Ao concluir esta atividade, o estudante será capaz de:

- Carregar dados de arquivos CSV usando pandas
- Inspecionar a estrutura e dimensões de um DataFrame
- Identificar e descrever colunas e seus tipos de dados
- Detectar valores nulos e duplicatas
- Gerar e interpretar estatísticas descritivas básicas
- Documentar suas descobertas em linguagem clara e acessível
