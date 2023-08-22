# Hadoop_Hive_GCP
Criação de um database no Hive e análise de dados a partir da criação de um cluster Hadoop via Dataproc no Google Cloud Platform (GCP).

<p align="center">
    <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%3Fid%3DOIP.hHKfkc_0Yga8QIH5_Niz6QHaE8%26pid%3DApi&f=1&ipt=7112616f576d210d50255b96d040f0ff50516566f2c332ef311cee0921c2e42e&ipo=images" alt="Hadoop">
</p>


### Este projeto envolveu:
- Criação de um cluster Hadoop via Dataproc no GCP;
- Criação de um dataset no hdfs e ingestão de CSVs no mesmo;
- Criação de um database no Hive;
- Criação de tabelas via jdbc no Hive;
- Ingestão de dados no Hive;
- Consultas em SQL via jdbc no Hive;
- Análise de Dados.

## Criação de um cluster Hadoop via Dataproc no GCP
Ambiente GCP 

![Cluster](https://i.imgur.com/uZx4VXN.png)

## Criação de um dataset no hdfs e ingestão de CSVs no mesmo
Feito por linha de comando e ingestão de três CSVs

![Hdfs](https://i.imgur.com/hHvdC62.png)

## Criação de um database no Hive
Criação do database de nome "database3"

![Hive](https://i.imgur.com/qmya7zb.png)

## Criação de tabelas via jdbc no Hive
Ao todo foram criadas três tabelas

![Jdbc](https://i.imgur.com/eZQYOoH.png)

## Ingestão de dados no Hive
A ingestão foi feita nas tabelas via jdbc
![Dados](https://i.imgur.com/P2PRHXj.png)

## Consultas em SQL via jdbc no Hive
Demonstração de uma dentre várias consultas feitas em SQL
![Select](https://i.imgur.com/M2vURnI.png)

## Análise de Dados

Os dados usados neste projeto são referentes a transações de cartões de crédito de cidadões estadunienses. Nesses CSV é possível encontrar informações sobre taxas de fraude, valores de compra, códigos de categoria de comerciante (MCCs) e outras métricas (o dicionários de dados está disponível no topo da página).

A análise de dados teve por objetivo responder as seguintes perguntas:
- Qual é o número médio de transações por dia da semana?
- Qual é o total de usuários por estado?
- Qual é a média de idade dos usuários por estado?
- Qual é o número médio de cartões emitidos por marca de cartão?
- Qual é o total de transações por ano e por mês?
- Qual é o número médio de cartões emitidos por tipo de cartão?
- Qual é o número de transações por estado do comerciante?
- Qual é o número médio de cartões de crédito por faixa etária?
- Qual é o total de transações por estado e por mês?

A obtenção das respostas foi possível graças as consultas realizadas em SQL (os scripts estão no topo da página). Os resultados foram:

-
-
-

Fonte dos dados:
Kaggle - https://www.kaggle.com/datasets/ealtman2019/credit-card-transactions?select=sd254_users.csv
