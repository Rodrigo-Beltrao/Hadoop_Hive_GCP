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

Os dados usados neste projeto são referentes a transações de cartões de crédito de cidadãos estadunidenses. Nesses CSV é possível encontrar informações sobre taxas de fraude, valores de compra, códigos de categoria de comerciante (MCCs) e outras métricas (o dicionário de dados está disponível no final da página).

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

A obtenção das respostas foi possível graças as consultas realizadas em SQL (os scripts com os resultados das consultas estão em uma pasta no topo da página). A partir dos resultados, foi possível tirar os seguintes insights:

- Insights extraídos do número médio de transações por dia da semana: 
   
Tendência de Atividade: A tendência geral de atividade parece mostrar uma alta nos primeiros dias do mês, uma queda gradual e um aumento novamente nos últimos dias. Isso pode estar relacionado a datas de pagamento de salários, quando os clientes têm mais recursos disponíveis.

Picos e Vales de Transações: Os dias 15, 2 e 1 apresentam os picos mais altos de transações, enquanto o dia 31 registra o menor número de transações. Esses padrões podem ser influenciados por datas de pagamento, compras recorrentes ou outros fatores sazonais.

- Insights extraídos do total de usuários por estado:

Centros Financeiros: Cidades com maior número de usuários, como Houston com 22 usuários, podem ser centros financeiros onde a emissão de cartões de crédito é mais comum devido à presença de instituições financeiras.

Necessidades de Marketing: Os dados podem ser usados para personalizar estratégias de marketing e ofertas de produtos com base nas características de uso de cartão de crédito em diferentes cidades.

- Insights extraídos da média de idade dos usuários por estado:

Venda de Serviços bancários: Com esses dados é possível direcionar serviços de planejamento de aposentadoria, consultoria de investimentos e opções de aposentadoria para cidades ondem há um usuários mais velhos e para o público mais jovens seria interessante direcionar programas de empréstimos para estudantes com taxas competitivas e opções flexíveis de pagamento, além de serviços bancários digitais, como aplicativos móveis, carteiras digitais e plataformas de pagamento online.

Cartões para o público correto: Serviços que oferecem cartões de crédito com recompensas direcionadas a categorias de consumo mais relevantes para jovens, como recompensas em compras online, streaming de mídia e alimentação, enquanto cartões de crédito com recompensas direcionadas a viagens e experiências podem atrair públicos mais velhos que desejam aproveitar seus anos de aposentadoria para explorar novos destinos. 

- Insights extraídos do número médio de cartões emitidos por marca de cartão:

Distribuição de Emissão de Cartões: As marcas de cartões de crédito listadas têm médias de emissão de cartões muito próximas entre si. As médias variam apenas ligeiramente, com diferenças de centésimos.

Competição Equilibrada: As marcas de cartões de crédito listadas (Amex, Discover, Mastercard, Visa) parecem estar em um estado de competição bastante equilibrada em termos de emissão de cartões.

Amex com Média Ligeiramente Maior: A marca "Amex" (American Express) apresenta a média de cartões emitidos um pouco mais alta do que outras marcas, embora a diferença seja pequena.

Estratégias de Marketing e Emissão de Cartões: Com base nas médias de cartões emitidos, as marcas de cartões de crédito podem ajustar suas estratégias de marketing e emissão de cartões para melhor atender às necessidades dos clientes.

- Insights extraídos do total de transações por ano e por mês:

Padrões Temporais: Pode-se observar padrões sazonais nas transações. Os números de transações parecem variar ao longo dos anos e meses, com algumas flutuações e tendências.

Crescimento e Declínio: Há meses em que o número de transações aumenta, como dezembro de 2004 (107 transações), ou diminui, como em março de 2009 (80 transações). Isso pode estar relacionado a fatores sazonais, feriados, eventos econômicos ou outras influências externas.

Ano de 2007: Parece que o ano de 2007 teve um padrão interessante, com os números de transações oscilando em torno dos 100 em muitos meses. Pode ser interessante investigar o que aconteceu nesse ano que levou a essa estabilidade.

Ano de 2016: O ano de 2016 parece ter um mês de junho com um número significativamente menor de transações (72). Isso poderia ser resultado de uma situação específica naquele mês.

Tendência de Alta e Baixa: Observando os números totais de transações ao longo dos anos, parece haver uma tendência geral de crescimento até 2018, seguida por uma tendência de queda nos anos subsequentes.

Avaliação de Desempenho: Esses dados podem ser usados para avaliar o desempenho de diferentes meses e anos em termos de transações. Isso poderia ajudar na tomada de decisões de negócios, como ajustes em estratégias de marketing ou planejamento financeiro.

Coronavírus (COVID-19) Impacto: O ano de 2020 parece ter menos dados disponíveis (apenas janeiro e fevereiro), o que pode estar relacionado ao início da pandemia de COVID-19 e suas consequências nas transações.

- Insights extraídos do número médio de cartões emitidos por tipo de cartão:

Variação Sutil: Embora haja uma pequena diferença nas médias, essa diferença não é tão significativa. Isso pode sugerir que a empresa emissora de cartões possui uma distribuição relativamente uniforme de emissão de diferentes tipos de cartões.

Cartões Pré-pagos: A média de emissão para "Debit (Prepaid)" é ligeiramente maior do que para os outros tipos. Isso pode indicar uma demanda crescente por cartões pré-pagos, possivelmente por pessoas que buscam controlar seus gastos ou não possuem acesso a crédito.

Tomada de Decisão: Com base nesses dados, a instituição financeira pode avaliar qual tipo de cartão tem maior demanda e considerar ajustes em suas estratégias de marketing ou oferta de produtos.

Segmentação de Mercado: Dependendo da estratégia da instituição financeira, pode haver oportunidades de segmentação de mercado com base nos diferentes tipos de cartão, considerando as preferências dos clientes.

- Insights extraídos do número de transações por estado do comerciante:

Centros Urbanos e Turísticos: Algumas cidades turísticas ou centros urbanos têm uma alta atividade de transações, como "Las Vegas" com 84 transações e "Los Angeles" com 54 transações.

Cidades Pequenas: Cidades menores, como "Lackland A F B" e "Lockney", têm menos transações, o que é esperado devido à sua natureza menos populosa.

Transações Online: A entrada "ONLINE" tem um grande número de transações (1.317), sugerindo a possibilidade de transações online ou digitais.

Identificação de Tendências: Com base nessas informações, é possível identificar as cidades mais ativas em termos de transações e também analisar padrões de comportamento de gastos em diferentes localidades.

- Insights extraídos do número médio de cartões de crédito por faixa etária:

Consistência no Número de Cartões: As médias do número de cartões emitidos são bastante consistentes entre as diferentes faixas etárias, variando de cerca de 706 a 711. Isso sugere que, em média, os usuários de todas as faixas etárias têm um número semelhante de cartões.

Participação Equitativa: Os dados sugerem que as faixas etárias 18-30, 31-45, 46-60 e 60+ têm uma participação relativamente equitativa no número médio de cartões emitidos.

Padrões de Uso de Cartão: A consistência nas médias pode indicar que a demanda por cartões e seu uso não variam significativamente com a idade. Isso pode refletir a adoção generalizada de cartões de crédito e débito em diferentes grupos etários.

Uso Financeiro Online: Dado que os números médios são bastante altos e consistentes em todas as faixas etárias, isso pode sugerir que os cartões são usados tanto para transações em lojas físicas quanto para transações online.

Necessidades Financeiras Diversificadas: Usuários de todas as faixas etárias têm um número semelhante de cartões, o que pode indicar que suas necessidades financeiras são diversas e podem incluir uma variedade de instituições financeiras, tipos de cartões e serviços.

- Insights extraídos do total de transações por estado e por mês:

Comportamento Anômalo: Alguns estados têm um número significativamente alto de transações em comparação com outros, como La Verne em janeiro e outubro. Pode haver razões específicas para esses picos, como promoções ou eventos locais.

Presença Online: A categoria "ONLINE" também aparece nos dados, indicando transações online. Ela tem um número considerável de transações, o que pode refletir a crescente preferência por compras online.

Atividade Mensal de Transações: Os dados podem sugerir que os padrões de transações não são constantes ao longo dos meses, e podem ser influenciados por fatores sazonais, eventos especiais, feriados e comportamentos do consumidor.

### Proposta de evolução do trabalho: Utilizar técnicas avançadas de aprendizado de máquina para desenvolver um modelo de detecção de fraude utilizando os dados disponíveis. O modelo poderá ser feito utilizando a linguagem de programação java com o Apache Mahout ou a partir da linguagem de programação python com bibliotecas de machine learning no jupyter notebook.

Fonte dos dados:
Kaggle - https://www.kaggle.com/datasets/ealtman2019/credit-card-transactions?select=sd254_users.csv



# Dicionário de Dados

## Tabela: user0_credit_card_transactions

| Coluna                  | Descrição                                       |
|-------------------------|-------------------------------------------------|
| chave                   | Chave única para a transação                    |
| card                    | Número do cartão de crédito utilizado na transação |
| year                    | Ano da transação                                |
| month                   | Mês da transação                                |
| day                     | Dia da transação                                |
| tempo                   | Horário da transação                            |
| amount                  | Valor da transação                              |
| use_chip                | Indica se o chip do cartão foi utilizado       |
| merchant_name           | Nome do estabelecimento comercial               |
| merchant_state          | Estado do estabelecimento comercial             |
| zip                     | Código postal do estabelecimento comercial      |
| mcc                     | Código de categoria do estabelecimento comercial |
| errors                  | Indica se ocorreram erros na transação          |
| is_fraud                | Indica se a transação é fraudulenta             |

## Tabela: sd254_users

| Coluna                  | Descrição                                       |
|-------------------------|-------------------------------------------------|
| person                  | Identificação única da pessoa                  |
| current_age             | Idade atual da pessoa                          |
| retirement_age          | Idade de aposentadoria da pessoa               |
| birth_year              | Ano de nascimento da pessoa                    |
| gender                  | Gênero da pessoa                               |
| address                 | Endereço da pessoa                             |
| apartment               | Número do apartamento da pessoa                |
| city                    | Cidade da pessoa                               |
| state                   | Estado da pessoa                               |
| zipcode                 | Código postal da pessoa                        |
| latitude                | Latitude da localização da pessoa              |
| longitude               | Longitude da localização da pessoa             |
| per_capita_income       | Renda per capita na região do CEP              |
| yearly_income           | Renda anual da pessoa                          |
| total_debt              | Dívida total da pessoa                         |
| fico_score              | Pontuação FICO da pessoa                       |
| num_credit_cards        | Número de cartões de crédito da pessoa         |

## Tabela: sd254_cards

| Coluna                  | Descrição                                       |
|-------------------------|-------------------------------------------------|
| chave2                  | Chave única para o cartão                      |
| card_index              | Índice do cartão                               |
| card_brand              | Marca do cartão                                |
| card_type               | Tipo do cartão                                 |
| card_number             | Número do cartão                               |
| expires                 | Data de expiração do cartão                    |
| cvv                     | Código de segurança do cartão                  |
| has_chip                | Indica se o cartão possui chip                |
| cards_issued            | Número de cartões emitidos para o usuário      |
| credit_limit            | Limite de crédito do cartão                    |
| acct_open_date          | Data de abertura da conta do cartão            |
| year_pin_last_changed   | Ano em que o PIN do cartão foi alterado        |
| card_on_dark_web        | Indica se o cartão está na Dark Web            |

