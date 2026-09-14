# Análise de Dados: Gagueira e Eventos de Disfluência

Projeto de análise de dados sobre gagueira utilizando o dataset **SEP-28k (Stuttering Events in Podcasts)**, com foco em tratamento de dados, análise exploratória, SQL, visualização no Power BI e, posteriormente, Machine Learning.

---

## Sobre o projeto

Este projeto utiliza o dataset **SEP-28k**, composto por milhares de trechos de fala de pessoas que gaguejam, extraídos de podcasts e classificados de acordo com diferentes tipos de eventos de disfluência.

O objetivo é explorar os dados para identificar padrões na ocorrência desses eventos, analisar sua distribuição e transformar os resultados em informações que possam ser visualizadas e interpretadas por meio de ferramentas de análise de dados.

O projeto será desenvolvido de forma progressiva, começando pelo tratamento e exploração dos dados e posteriormente avançando para consultas em SQL, criação de um dashboard no Power BI e aplicação de técnicas de Machine Learning para classificação dos eventos de disfluência.

Além do interesse técnico, o tema possui uma motivação pessoal: a gagueira também faz parte da minha experiência. A escolha do problema surgiu como uma oportunidade de aplicar conhecimentos de dados e tecnologia a um tema que conheço de forma pessoal.

---

## Dataset

O projeto utiliza o **SEP-28k (Stuttering Events in Podcasts)**, um dataset desenvolvido para pesquisas relacionadas à detecção automática de eventos de gagueira em fala.

Os trechos de áudio possuem anotações relacionadas a diferentes tipos de eventos de disfluência, incluindo:

* **Block** — bloqueios durante a fala
* **Prolongation** — prolongamentos de sons
* **Sound Repetition** — repetição de sons
* **Word Repetition** — repetição de palavras
* **Interjection** — interjeições

O dataset também possui informações relacionadas aos episódios e aos participantes, permitindo diferentes possibilidades de análise.

---

## Estrutura do projeto

```text
stuttering-data-analysis/
├── archive/                         # Arquivos originais do dataset
├── notebooks/
│   ├── exploracao_dados.ipynb       # Exploração inicial dos dados
│   ├── limpeza_tratamento.ipynb     # Limpeza e preparação dos dados
│   └── analise.ipynb                # Análises exploratórias
├── sql/                             # Consultas e análises utilizando SQL
├── powerbi/                          # Arquivos e documentação do dashboard
├── machine_learning/                 # Modelos de classificação
├── README.md                         # Documentação do projeto
└── notas_de_projeto.md              # Anotações e decisões técnicas
```

---

## Tecnologias utilizadas

* **Python**
* **Pandas** — tratamento, transformação e análise dos dados
* **NumPy** — operações e manipulação numérica
* **Matplotlib** — visualização de dados
* **Jupyter Notebook** — exploração e documentação
* **SQL** — consultas e análises dos dados
* **Power BI** — criação do dashboard
* **Scikit-learn** — Machine Learning
* **Librosa** — processamento e extração de características dos áudios

---

## Etapas do projeto

### 1. Carregamento e entendimento dos dados

* [x] Carregar os arquivos de labels
* [x] Carregar os arquivos de episódios
* [x] Consolidar os arquivos em DataFrames
* [ ] Identificar as relações entre as tabelas
* [ ] Documentar a estrutura do dataset
* [ ] Avaliar quantidade de registros e variáveis
* [ ] Identificar valores ausentes e inconsistências

### 2. Tratamento dos dados

* [ ] Padronização dos nomes e tipos das colunas
* [x] Tratamento de valores ausentes (não possui)
* [x] Identificação de registros duplicados (não possui)
* [ ] Validação das relações entre episódios, falas e labels
* [ ] Criação da base final para análise
* [ ] Documentação das decisões de tratamento

### 3. Análise exploratória

* [ ] Analisar a distribuição dos eventos de disfluência
* [ ] Comparar os diferentes tipos de eventos
* [ ] Analisar a quantidade de falas por episódio
* [ ] Analisar a distribuição entre participantes
* [ ] Analisar características dos episódios
* [ ] Explorar a duração dos trechos de áudio
* [ ] Identificar possíveis padrões nos dados
* [ ] Criar visualizações para os principais indicadores
* [ ] Documentar os principais insights

### 4. SQL

* [ ] Criar estrutura das tabelas
* [ ] Importar os dados para o banco
* [ ] Realizar consultas de agregação
* [ ] Utilizar `JOIN` entre as tabelas
* [ ] Analisar a frequência dos eventos
* [ ] Criar consultas para indicadores do projeto
* [ ] Utilizar funções de janela quando necessário
* [ ] Documentar as principais consultas

### 5. Power BI

* [x] Importar os dados tratados
* [x] Modelar os dados
* [ ] Criar relacionamentos
* [ ] Criar medidas e indicadores
* [ ] Criar análise da distribuição dos eventos
* [ ] Criar filtros e segmentações
* [ ] Criar dashboard
* [ ] Organizar e refinar os visuais
* [ ] Revisar o dashboard

### 6. Machine Learning

Após a conclusão das etapas de análise exploratória, os dados serão utilizados para investigar a possibilidade de classificação automática dos diferentes eventos de disfluência.

* [ ] Definir o problema de classificação
* [ ] Preparar os dados para Machine Learning
* [ ] Explorar características dos áudios
* [ ] Extrair características utilizando processamento de áudio
* [ ] Criar baseline
* [ ] Treinar modelos de classificação
* [ ] Avaliar Precision, Recall e F1-score
* [ ] Criar matriz de confusão
* [ ] Comparar diferentes modelos
* [ ] Documentar os resultados

---

## Análises planejadas

O projeto pretende responder perguntas como:

* Qual é o tipo de evento de disfluência mais frequente?
* Como os diferentes tipos de eventos se distribuem?
* Existem episódios com maior concentração de determinados eventos?
* Como os eventos se distribuem entre os participantes?
* Qual é a duração média dos trechos analisados?
* Existem padrões relevantes entre as características dos áudios e os eventos classificados?
* Quais características apresentam maior relação com cada tipo de disfluência?
* É possível utilizar Machine Learning para classificar automaticamente diferentes eventos de gagueira?

As perguntas poderão ser ampliadas conforme novos padrões forem identificados durante a análise.

---

## Power BI

O projeto contará com um dashboard desenvolvido no Power BI para apresentar os principais indicadores e padrões encontrados durante a análise.

Entre os possíveis indicadores estão:

* Total de falas analisadas
* Total de episódios
* Quantidade de participantes
* Distribuição dos eventos de disfluência
* Frequência de cada tipo de evento
* Duração dos trechos analisados
* Comparações entre diferentes categorias

**Status:** Em desenvolvimento.

---

## Machine Learning

A etapa de Machine Learning será desenvolvida posteriormente à análise exploratória.

O objetivo não é realizar diagnóstico de gagueira, mas investigar a possibilidade de **classificar automaticamente diferentes eventos de disfluência presentes nos áudios**.

Os modelos serão avaliados utilizando métricas apropriadas para classificação, considerando especialmente possíveis diferenças na distribuição das classes.

---

## Motivação

A escolha deste projeto possui também uma motivação pessoal.

A gagueira faz parte da minha própria experiência, e isso despertou meu interesse em utilizar conhecimentos de **Análise de Dados, Machine Learning e tecnologia** para estudar um problema relacionado à fala.

O objetivo é transformar essa motivação em um projeto tecnicamente estruturado, utilizando dados reais e ferramentas aplicadas ao mercado de dados.

---

## Objetivo profissional

Este projeto também faz parte da minha evolução na área de **Dados**, reunindo diferentes etapas do processo de análise:

```text
Dados brutos
    ↓
Python / Pandas
    ↓
Tratamento
    ↓
Análise exploratória
    ↓
SQL
    ↓
Power BI
    ↓
Machine Learning
```

A proposta é demonstrar, em um único projeto, a capacidade de trabalhar desde a preparação e análise dos dados até a criação de visualizações e experimentos de Machine Learning.

---

## Autor

**Enuk Nogueira**

Estudante de **Big Data e Inteligência Analítica**, com interesse em **Análise de Dados, Business Intelligence, Data Science e Machine Learning**.
