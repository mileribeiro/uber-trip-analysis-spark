# Análise de Corridas da Uber com Apache Spark (PySpark)

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mileribeiro/uber-trip-analysis-spark/blob/main/uber_trip_analysis_spark.ipynb)

Este projeto apresenta uma **análise exploratória de dados de corridas da Uber utilizando Apache Spark (PySpark)**.  
O objetivo é demonstrar como ferramentas de processamento distribuído podem ser utilizadas para **carregar, transformar e analisar dados de mobilidade em escala**.

A análise foi desenvolvida em **Google Colab**, utilizando a API do **PySpark** para manipulação e agregação dos dados.

---

# Tecnologias Utilizadas

- Python
- Apache Spark
- PySpark
- Google Colab

---

# Dataset

O dataset utilizado contém informações sobre corridas realizadas em uma plataforma de mobilidade, incluindo variáveis como:

- **Booking Status** – status da corrida  
- **Booking Value** – valor total da corrida  
- **Ride Distance** – distância percorrida  
- **Vehicle Type** – tipo de veículo utilizado  
- **Driver Ratings** – avaliação do motorista  
- **Customer Rating** – avaliação do passageiro  

Essas informações permitem realizar análises relacionadas a **comportamento das corridas, padrões de distância e estrutura de preços**.

---

# Etapas da Análise

O notebook segue um fluxo estruturado de análise de dados:

### 1. Inicialização do Apache Spark
Criação da sessão principal do Spark para processamento distribuído dos dados.

### 2. Carregamento do Dataset
Leitura do arquivo CSV utilizando PySpark e inspeção inicial da estrutura dos dados.

### 3. Inspeção do Schema
Verificação dos tipos de dados inferidos pelo Spark e identificação de inconsistências.

### 4. Tratamento e Conversão de Tipos
Substituição de valores `"null"` e conversão das colunas para tipos numéricos apropriados.

### 5. Criação de Variáveis Derivadas
Construção da variável **price_per_km**, que representa o preço por quilômetro da corrida.

### 6. Filtragem de Corridas Concluídas
Para algumas análises, foram consideradas apenas corridas com status **Completed**, garantindo maior consistência nos cálculos.

### 7. Análise Exploratória
Foram realizadas análises agregadas para identificar padrões nos dados, incluindo:

- Valor médio das corridas por tipo de veículo
- Distância média das corridas por tipo de veículo
- Preço médio por quilômetro

---

# Principais Insights

A análise exploratória revelou alguns padrões interessantes:

- O **preço por quilômetro tende a diminuir em corridas mais longas**, possivelmente devido à presença de uma taxa base na estrutura de preços.
- A **distância média das corridas é bastante semelhante entre os diferentes tipos de veículo**.
- O **tipo de veículo não parece influenciar significativamente a distância das viagens** no dataset analisado.

---

# Como Executar o Projeto

O notebook pode ser executado de duas formas:

### Google Colab
Basta abrir o notebook diretamente no Colab.

### Ambiente Local
Instalar as dependências necessárias:
pip install pyspark


---

## Autor

Milena Vasconcelos Ribeiro
