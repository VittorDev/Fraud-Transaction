# Fraud-Transaction
# Introdução ao problema
Em muitos setores, como bancos, e-commerces e seguros, a fraude é um problema sério e pode causar grandes prejuízos financeiros, impactando negativamente a confiança dos clientes desses setores. O objetivo de um sistema de detecção de fraudes é identificar transações ou atividades fraudulentas com a maior precisão possível, minimizando transações que possam ser verdadeiras mas não são, e transações legítimas que são incorretamente classificadas como fraudulentas.

Um dos desafios na detecção de fraudes é que os dados geralmente são altamente desbalanceados, com a maioria das transações sendo legítimas e apenas uma pequena porcentagem sendo fraudulentas. Além disso, os fraudadores estão constantemente adaptando suas táticas, o que torna o problema dinâmico e em constante evolução.

Neste contexto, temos dois conjuntos de dados: um de treino (fraudTrain.csv) e outro de teste (fraudTest.csv). O objetivo é desenvolver um modelo preditivo capaz de identificar transações suspeitas com base em um conjunto de características fornecidas, utilizando o conjunto de treino para construir o modelo e o conjunto de testes para avaliar seu desempenho.

# Objetivo
O objetivo principal deste projeto é desenvolver e avaliar modelos preditivos capazes de identificar transações fraudulentas de maneira eficaz e eficiente. Especificamente, buscamos:

1 - Identificar e selecionar as características mais relevantes que ajudam a diferenciar transações legítimas de fraudulentas.

2- Explorar e comparar diferentes técnicas de aprendizado de máquina para a detecção de fraudes.

3 - Desenvolver estratégias para lidar com o problema do desbalanceamento de classes no dataset.

4- Minimizar a taxa de falsos positivos e falsos negativos, otimizando assim a eficiência do modelo na detecção de fraudes.

Esses objetivos servirão como base para criar um sistema de detecção de fraudes que possa ser implementado em cenários reais para prevenir perdas financeiras e proteger a integridade das transações.

# 1 - Importação dos Dados

# 2 - Dicionário de Colunas
Para um melhor entendimento do que cada uma das categórias significa no contexto da análise, é necessário um dicionário de cada uma das colunas.
1. trans_date_trans_time: The date and time of the transaction (A data e hora em que ocorreu a transação)
2. cc_num: credit card number (Número do cartão de crédito)
3. merchant: Merchant who was getting paid (Estabelecimento que recebeu o pagamento)
4. category: In what area does that merchant deal (Qual é a categoria que se enquadra o estabelecimento)
5. amt: Amount of money in American Dollars (Valor em dollars da transação)
6. first: first name of the card holder (Dados do primeiro nome do detentor do cartão)
7. last: last name of the card holder (Dados do último nome do detentor do cartão)
8. last: last name of the card holder (Dados do gênero do detentor do cartão)
9. street:Street of card holder residence (Rua em que reside o detentor do cartão)
10. city:city of card holder residence (Cidade em que reside o detentor do cartão)
11. state:state of card holder residence (Estado em que reside o detentor do cartão)
12. zip:ZIP code of card holder residence (O código da residência do detentor do cartão)
13. lat:latitude of card holder (Dados de geolocalização do dentetor do cartão)
14. long:longitude of card holder (Dados de geolocalização do dentetor do cartão)
15. city_pop:Population of the city (Dados da população da cidade onde o dentetor do cartão habita)
16. ob:trade of the card holder (Ocupação profissional do dententor do cartão)
17. ob:Date of birth of the card holder (Data de nascimento do detentor do cartão)
18. trans_num: Transaction ID (Identificação da transação em questão)
19. unix_time: Unix time which is the time calculated since 1970 to today
20. merch_lat: latitude of the merchant (Dados de geolocalização do estabelecimento alvo da transação)
21. merch_long:longitude of the merchant (Dados de geolocalização do estabelecimento alvo da transação)
22. is_fraud: Whether the transaction is fraud(1) or not(0) (Varíavel alvo, onde o 0 é não fraude e 1 é operações fraudelentas)

O Data set é composto por 22 colunas e 1.852.394 linhas de dados.

# Preperação dos Dados

# Análise Exploratória
ANÁLISES UNIVARIADAS

Iremos começar a análise analisando cada varíavel, para conhecermos mais profundamente as observações do nosso dataset e visando responder as seguintes perguntas:

1 - Quantidade de observações de fraudes e não fraudes

2 - Gênero que mais possuí recorrência de fraudes

3 - Idade em que mais ocorre fraudes
