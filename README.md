# Tratamento-dados-INSS-CAT---Pandas-PySpark
Projeto realizado para Bootcamp de Engenharia de Dados da SoulCode, utilizando Pandas, PySpark, Google Cloud Storage, MongoDB e MySQL.


## Sobre a base de dados: 
Disponibilização dos dados de CAT, cadastradas no sistema informatizado de Comunicação de Acidentes do Trabalho do INSS (CATWEB) ou quando da concessão de benefício por incapacidade acidentário, observado o disposto no Decreto nº 8.777/16 e Lei de Acesso à Informação nº 12.527/2011.

* As bases disponibilizadas contém o ano de 2022 separadas por meses (coluna de controle);
* As informações foram colhidas por sistema, telefone e ou presencialmente - sendo então provável existirem dados divergentes ou ausentes (faltantes).

## Instruções:


Nivel Infra
* O arquivo original e tratado deve ser salvo em MongoDB Atlas em coleções diferentes (enumerar com o final trat ou orig)
* Os Datasets devem ser obrigatoriamente salvos em uma bucket do Google CloudStorage (original e tratado)
* Disponibilizar o dataset final em um servidor MySQL

Nivel Pandas
* Realizar a extração correta para um dataframe.
* Verificar a existência de dados inconsistentes e realizar a limpeza para NaN/NA ou algum valor atribuído por você explicando o porque da decisão.
* Realizar o drop (se necessário) de colunas do dataframe realizando o comentário do porque da exclusão 
* Todos os passos devem ser comentados (exclusivos)
* Agregar todos os DF's originais em um unico DF tratado
* Criar no mínimo 3 insights dos dados apresentados podendo ser construído com auxilio de plots

Nivel PySpark
* Deverá ser montada a estrutura do DataFrame utilizando o StructType.
* Verificar a existência de dados inconsistentes, nulos e realizar a limpeza.
* Verificar a necessidade de drop em colunas ou linhas. Caso seja necessário, fazer comentário do porque.
* Realizar a mudança de nome de pelo menos 2 colunas
* Deverá criar pelo menos duas novas colunas contendo alguma informação relevante sobre as outras colunas já existentes (Funções de Agrupamento, Agregação ou Joins). (Use a sua capacidade analítica)
* Deverá utilizar filtros, ordenação e agrupamento, trazendo dados relevantes para o negócio em questão. (Use a sua capacidade analítica)
* Utilizar pelo menos duas Window Functions
* 5 insights utilizando SparkSQL
