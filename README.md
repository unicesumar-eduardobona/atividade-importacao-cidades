### Atividade de Estudo
# Importação de Estados e Cidades

Imagine que recebeu de sua equipe a missão simples
de criar estas tabelas e importar os registros no 
banco e para esta atividade irá usar seus
conhecimentos em PHP e PDO para fazer
a criação destas tabelas e posteriormente
a importação dos dados.

Apenas para constar, sua equipe disse que em média
um desenvolvedor iniciante resolveria este 
desafio em 4 horas no máximo e que o mais
importante é que o banco de dados esteja OK não importando
muito o código, que posteriormente será jogado fora.

**Diante disso, desenvolva um script.php que atenda
aos requisitos abaixo (recebido de sua equipe)**

## Requisitos

1. criar uma tabela chamada estado com os campos
    - cod_uf varchar(2) chave primária
    - cod_ibge int
    - nome_estado varchar(255)
    - nome_regiao varchar(255)
    - quantidade_cidades (int)
    - **todos estes campos com valores obrigatórios**

2. importar para a tabela estado todos os registros
contidos no arquivo lista_estados.csv

3. criar uma tebela chamada municipio com os campos
    - cod_ibge int chave primária
    - cod_uf varchar(2) chave estrangeira tabela estado
    - nome_municipio
    - nome_regiao
    - quantidade_populacao
    - tipo_porte
    
4. importar para a tabela municipio todos os registros
contidos no arquivo lista_municipios.csv

#### Algumas dicas

- Um dos integrantes da sua equipe já lhe enviou
um artigo escrito por um desenvolvedor PHP
que aponta várias formas de se ler um arquivo de texto
e [este artigo está disponível na url](https://blog.vivaweb.net/2020/08/04/ao-ler-um-arquivo-de-texto-com-php-voce-sabe-qual-codigo-adotar)

- Outro integrante da sua equipe já lhe adiantou que
o formato do arquivo a ser lido é do tipo .CSV
e que o PHP tem uma função que transforma string do tipo csv
em um array e [um exemplo pode ser encontrado no Manual do PHP](https://www.php.net/manual/en/function.str-getcsv.php)


Fontes:

- [Artigo Vivaweb](https://blog.vivaweb.net)
- [Manual do PHP](https://php.net)
- [Rede SUAS](http://blog.mds.gov.br/redesuas/lista-de-municipios-brasileiros/)