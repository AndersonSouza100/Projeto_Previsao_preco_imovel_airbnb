### Projeto_Previsao_preco_imovel_airbnb
## Contexto
No Airbnb, qualquer pessoa que tenha um quarto ou um imóvel de qualquer tipo (apartamento, casa, chalé, pousada, etc.) pode ofertar o seu imóvel para ser alugado por diária.
Você cria o seu perfil de host (pessoa que disponibiliza um imóvel para aluguel por diária) e cria o anúncio do seu imóvel.
Nesse anúncio, o host deve descrever as características do imóvel da forma mais completa possível, de forma a ajudar os locadores/viajantes a escolherem o melhor imóvel para eles (e de forma a tornar o seu anúncio mais atrativo)
Existem dezenas de personalizações possíveis no seu anúncio, desde quantidade mínima de diária, preço, quantidade de quartos, até regras de cancelamento, taxa extra para hóspedes extras, exigência de verificação de identidade do locador, etc.
## Nosso objetivo
Construir um modelo de previsão de preço que permita uma pessoa comum que possui um imóvel possa saber quanto deve cobrar pela diária do seu imóvel.
Ou ainda, para o locador comum, dado o imóvel que ele está buscando, ajudar a saber se aquele imóvel está com preço atrativo (abaixo da média para imóveis com as mesmas características) ou não.
As bases de dados foram retiradas do site kaggle: https://www.kaggle.com/allanbruno/airbnb-rio-de-janeiro. A IDE usada para desenvolver as linhas de código foi o Jupyter. O projeto em si já é bem autoexplicativo.

Antes de você rodar este projeto no seu computador, é importante entrar na pasta 'dataset' e extrair todos os arquivos, pois, eles são a base de dados original e sem tratamento do projeto. Extraia-os para a pasta 'dataset'. A seguir, falarei sobre cada arquivo contido neste trabalho:

1 - Projeto_Previsao_preco_imovel_airbnb.ipynb: esse é o arquivo principal do projeto, onde nele é realizado todo trabalho de Ciência de Dados. Está dividido em 8 passos:

      1 - Entendimento da área.
      2 - Entendimento do desafio.
      3 - Extração/Obtenção de Dados.
      4 - Ajustes dos dados (Limpeza dos Dados).
      5 - Análise Exploratória e Tratamento de Outliers.
      6 - Modelagem + Algoritmos.
      7 - Interpretação dos Resultados.
      8 - Deploy do Projeto.
Após a etapa 8, foram criados 2 arquivos: 'dados.csv' (que é nossa base de dados completa e tratada) e 'modelo.joblib' (que é o nosso modelo de inteligência artificial salvo em arquivo para facilitar sua leitura na hora do deploy). Este último arquivo que eu mencionei , ele também está neste projeto . Basta acessar a pasta 'modelo.joblib comprimido' e extrair todos os arquivos para a própria pasta. É importante que você coloque o arquivo 'modelo.joblib' na pasta inicial deste projeto.

2 - DeployProjetoAirbnb.ipynb: esse é o arquivo onde gerará uma tela para que o usuário possa colocar as informações do imóvel e prever o seu preço. Esse arquivo irá ler os dois arquivos gerados na etapa 8 do Deploy.

3 - DeployProjetoAirbnb.py: esse arquivo é a tela final onde o usuário irá colocar as informações do imóvel para prever o seu preço. Foi gerado pelo arquivo 2 e para que ele funcione, é necessário seguir o passo a passo:

      1 - abra no seu computador o Anaconda Prompt.
      2 - execute o comando: cd C:\Users\AndersonPC\Documents\GitHub\Projeto_Previsao_preco_imovel_airbnb 
      Observação: no passo 2 você deve colocar o caminho exato da pasta onde está o seu projeto. No meu caso está desta forma, mas no seu estará diferente.
      3 - execute o comando: streamlit run DeployProjetoAirbnb.py
      4 - Abrirá uma aba no seu navegador, basta colocar as informações do imóvel e clicar no botão 'Prever valor do imóvel'.

4 - primeiros_registros.csv: esse arquivo foi gerado durante o projeto para ter uma visualização melhor das colunas e fazer uma análise qualitativa. 

