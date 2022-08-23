# Shark Attack

  Project status(Completed)

# Objetivo do Projeto

  Para esse projeto utilizei a base de dados de Ataques de tubarão disponibilizada no link: https://www.kaggle.com/datasets/teajay/global-shark-attacks 
  projeto tinha como objetivo a limpeza do maximo de colunas possiveis da base de dados para responder uma 'Perguna' de negocios.
  
  A pergunta escolhida foi: Seriam os tubarões a reencarnação dos povos Celtas?
  
  Durante os dias 30 de outubro e 02 de novembro ocorre o Samhain, o solsticio de Outono no hemisfério norte. Logo, se os casos de ataque dos tubarões 
  for maior entre esses dias existe a possibilidade destes ataques serem um sacrificio para o Deus Tubarão. 
  
# Metodos

  Para o projeto utilizei os metodos de:
  - Data Filtering
  - Data Cleaning
  - String Methods
  - Regex
  - to.Datetime 
 
# Tecnologias 

  - Python
  - Pandas
  - MS Excel
  
# Descrição do Projeto

  - O dataset cru possuia 23 Colunas e 25722 linhas. A principio criei um DataFrame por meio do Pandas, removi todas as linhas duplicadas e nulas do dataset, pois para responder minha pergunta utilizei apenas as Colunas de 'Case Number' e 'Country'.
  - Na coluna 'Case Number' utilizei os metodos de str.replace, str.endswith, str.startswith e mascaras pra limpar a coluna de todos os dados irrelevantes
  - Na coluna 'Country' criei uma lista com todas as entradas não correrspondentes aos países do Hemisferio Norte e realizei uma manipulação do dataframe para localizar todos as 'chaves' da lista. Utilizei os metodos .loc e .drop para localizar as chaves na coluna e depois retira-las.
  - Após as manipulações o dataset finalizou com 26 Colunas e 2821 linhas, exportei o arquivo para o formato CSV e finalizei a analise filtrando os 3 dias selecionados para comparar com o total de ataques no periodo completo.

# Conclusão
  Dado que ataques de tubarão sempre aconteceram e vão continuar acontecendo, consideramos a população como infinita e não podemos fazer uma inferencia estatistica adequada.
  Entre os 2821 ataques catalogados no Hemisferio norte nos ultimos 120 anos apenas 25 casos ocorreram no periodo do Samhain, o que demostra a hipotese dos tubarões serem a reencarnação do povoado Celta inconclusiva. 
  
  
