# Análise de Viagens da Uber com Apache Spark

Este projeto apresenta uma análise exploratória de dados de viagens da Uber usando **Apache Spark (PySpark)**.

O objetivo é demonstrar como o processamento de dados distribuído pode ser aplicado para analisar conjuntos de dados de mobilidade e extrair insights operacionais.

---

## Tecnologias

- Apache Spark
- PySpark
- Google Colab
- Python

---

## Conjunto de Dados

O conjunto de dados contém informações sobre reservas de viagens, incluindo:

- Status da Reserva
- Valor da Reserva
- Distância da Viagem
- Tipo de Veículo
- Avaliações do Motorista
- Avaliações do Cliente

---

## Análises Realizadas

O notebook inclui as seguintes análises:

- Carregamento de dados usando Spark
- Inspeção de esquema
- Limpeza e conversão de tipos de dados
- Engenharia de recursos
- Cálculo do preço por quilômetro
- Análise agregada por tipo de veículo
- Análise da distância da viagem

---

## Principais Insights

Algumas observações da análise:

- O preço por quilômetro tende a diminuir à medida que a distância da viagem aumenta. - A distância média percorrida é semelhante entre diferentes tipos de veículos.

- O tipo de veículo não influencia significativamente a distância da viagem neste conjunto de dados.

---

## Executando o Notebook

O notebook pode ser executado usando o **Google Colab** ou qualquer ambiente Spark local.

---

## Autor

Milena Vasconcelos Ribeiro
