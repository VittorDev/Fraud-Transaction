# Fraud-Transaction
Este estudo tem como objetivo elaborar um modelo de machine learning capaz de prever transações fraudulentas, e entender quais os fatores contribuem para conseguir identificar uma transação fraudelenta.

O dataset utilizado para esse estudo será o "fraud transactions dataset" que reune dados de operações fraudelentas e não fraudelentas.

Esse dataset foi retirado do Kaggle, e pode ser acessado através deste link: https://www.kaggle.com/search?q=fraud+transaction+in%3Adatasets.

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

