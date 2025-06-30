# Projeto de Análise de Dados - Resultados Históricos do Futebol Internacional

**Autor:** Thomaz Colalillo Navajas
**Professor:** Fabio Gomes Jardim
**Disciplina:** Distributed Data Processing & Storage
**Data:** 30/06/2025

---

### 1. Objetivo do Projeto

Este projeto realiza uma análise exploratória sobre um dataset histórico de resultados de partidas de futebol entre seleções, desde a primeira partida oficial em 1872. O objetivo é utilizar PySpark em um ambiente Databricks para extrair insights, estatísticas e curiosidades sobre a história do esporte.

A análise busca responder a perguntas como:
*   Quais seleções jogaram mais partidas ao longo da história?
*   Qual o saldo de gols das principais seleções?
*   Qual a influência de jogar em casa vs. em campo neutro nos resultados?
*   Quais foram as maiores goleadas registradas?
*   Como o número de gols por partida evoluiu ao longo do tempo?

### 2. Dataset

O dataset utilizado, `results.csv`, é uma compilação de resultados de partidas de futebol entre seleções nacionais. Ele contém dados detalhados de cada partida, incluindo placares, torneios e locais.

As colunas do dataset são:
*   `date`: Data em que a partida foi realizada.
*   `home_teamName`: Nome da seleção que jogou em casa.
*   `away_teamName`: Nome da seleção visitante.
*   `home_scoreHome`: Gols marcados pela seleção da casa.
*   `away_scoreAway`: Gols marcados pela seleção visitante.
*   `tournamentName`: Nome do torneio ou competição (ex: "Friendly", "FIFA World Cup").
*   `cityCity`: Cidade onde a partida foi realizada.
*   `countryCountry`: País onde a partida foi realizada.
*   `neutralTRUE`: Campo booleano (`True`/`False`) que indica se a partida ocorreu em campo neutro.

### 3. Tecnologias Utilizadas

*   **Plataforma:** Databricks
*   **Linguagem:** Python
*   **Bibliotecas Principais:**
    *   **PySpark:** Para manipulação e análise distribuída dos dados.
    *   **Pandas:** Utilizado como ponte para carregar os dados a partir da web para um DataFrame Spark.
    *   **Requests:** Para realizar a chamada HTTP e baixar o dataset diretamente do GitHub.

### 4. Como Executar a Análise

Este repositório foi estruturado para garantir a reprodutibilidade do código sem a necessidade de configurações manuais por parte do usuário.

1.  **Importar o Notebook:** Faça o download do arquivo de notebook (`.ipynb` ou `.py`) deste repositório e importe-o para o seu ambiente Databricks.
2.  **Executar o Código:** Anexe o notebook a um cluster ativo e execute todas as células (`Run All`).

O notebook foi programado para **baixar o dataset `results.csv` diretamente deste repositório do GitHub**, não sendo necessário nenhum upload manual de arquivos para o DBFS (Databricks File System).

---

*Este repositório serve como entrega para o projeto da disciplina de Distributed Data Processing & Storage do curso de Engenharia de Dados da Faculdade de Informática e Administração Paulista (FIAP).*
