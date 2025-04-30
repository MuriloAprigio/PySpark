# 📈 🐍PySpark - Análise de Dados com Spark

## Repositório dedicado ao aprendizado e prática de manipulação e análise de dados utilizando PySpark.

Este repositório contém notebooks e scripts PySpark que demonstram diversas operações e funcionalidades da biblioteca Spark para processamento de dados em larga escala.

#### Fundamentos de DataFrames:

-   **Criar DataFrame / Ler Arquivo:** Demonstra como criar DataFrames do Spark a partir de diferentes fontes de dados, como arquivos CSV, Parquet, etc.
-   **Exibir DataFrame:** Métodos para visualizar o conteúdo e o esquema de um DataFrame.
-   **Verificar Tipos de Colunas:** Como inspecionar os tipos de dados de cada coluna em um DataFrame.
-   **Verificando Dados Nulos:** Técnicas para identificar e contar valores nulos em um DataFrame.
-   **Selecionar Colunas:** Formas de selecionar colunas específicas de um DataFrame.
-   **Selecionar Colunas com ALIAS:** Como renomear colunas durante a seleção.
-   **Organizar Select:** Ordenação dos resultados de uma seleção.
-   **Filtrar DataFrame:** Aplicação de filtros para selecionar linhas com base em condições.
-   **Filtrar DataFrame com 2 ou mais condições (AND / &):** Utilização do operador lógico AND para combinar múltiplos critérios de filtro.
-   **Filtrar DataFrame com 2 ou mais condições (OR / |):** Utilização do operador lógico OR para aplicar múltiplos critérios de filtro.
-   **Filtrar DataFrame combinando & e | (And e OR):** Demonstração de como usar AND e OR juntos para filtros complexos.
-   **Criar novas colunas (usando função lit):** Adição de novas colunas com valores literais.
-   **Criar coluna condicional (usando função substring):** Criação de colunas com base em substrings de outras colunas.
-   **Criar coluna condicional (usando função concat\_ws):** Criação de colunas concatenando outras colunas com um separador.
-   **Renomear Colunas:** Métodos para alterar os nomes das colunas em um DataFrame.
-   **Alterar tipo de coluna:** Conversão do tipo de dados de uma ou mais colunas.
-   **Drop de Colunas:** Remoção de colunas específicas de um DataFrame.

#### Window Ranking Functions:

-   **Window Function 1 - Numero de linhas - `row_number()`:** Atribuição de um número sequencial a cada linha dentro de uma janela.
-   **Window Function 2 - Ranking 1 - `rank()`:** Atribuição de ranks com lacunas quando há valores iguais.
-   **Window Function 3 - Ranking 2 - `dense_rank()`:** Atribuição de ranks sem lacunas, mesmo quando há valores iguais.
-   **Window Function 4 - Porcentagem Ranking - `percent_rank()`:** Cálculo da classificação relativa de cada linha dentro de uma janela.
-   **Window Function 5 - Divisão em ' N ' partes - `ntile()`:** Divisão das linhas de cada janela em 'N' grupos aproximadamente iguais.

#### Window Analytic Functions (Funções analíticas):

-   **Window Function 6 - LAG / Degrau - `lag()`:** Acesso aos valores de uma linha anterior dentro de uma janela.
-   **Window Function 7 - Lead / Degrau - `lead()`:** Acesso aos valores de uma linha seguinte dentro de uma janela.
-   **Window Function 8 - Função de agregação usando Window Function:** Aplicação de funções de agregação (como `sum`, `avg`, etc.) dentro de janelas.

#### Agregações:

-   **`GroupBy` + `AGG` 1:** Agrupamento de dados e aplicação de funções de agregação.
-   **`Where`:** Aplicação de filtros após o agrupamento.
-   **`Describe`:** Obtenção de estatísticas descritivas sobre as colunas de um DataFrame.
-   **`Collect()`:** Coleta dos dados do DataFrame para o driver (usar com cautela em DataFrames grandes).
-   **`When()` / `Otherwise()`:** Implementação de lógica condicional na criação ou transformação de colunas.

#### União e Joins:

-   **`Union` (Concat):** Combinação de dois DataFrames com a mesma estrutura.
-   **Join - Simples:** Operação básica de junção entre dois DataFrames.
-   **Inner Join:** Retorna apenas as linhas que possuem correspondência em ambas as tabelas.
-   **Left Join:** Retorna todas as linhas da tabela esquerda e as correspondentes da tabela direita (com valores nulos onde não há correspondência).
-   **Right Join:** Retorna todas as linhas da tabela direita e as correspondentes da tabela esquerda (com valores nulos onde não há correspondência).
-   **Full Join:** Retorna todas as linhas de ambas as tabelas, com valores nulos onde não há correspondência.
-   **Semi Join:** Retorna as linhas da tabela esquerda que possuem correspondência na tabela direita (apenas as colunas da esquerda são mantidas).
-   **Anti Join:** Retorna as linhas da tabela esquerda que não possuem correspondência na tabela direita (apenas as colunas da esquerda são mantidas).

Explore os notebooks e scripts para ver exemplos práticos de cada uma dessas operações em PySpark!
