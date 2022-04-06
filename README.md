# SQL_Udemy
Informações retiradas dos slides da aula da udemy

## Modelagem Conceitual, Lógica e Física
Os modelos de banco de dados são usados para descrever, mais detalhadamente, a estrutura de um banco de dados. Eles servem como parte importante da documentação dos sistemas que auxiliam os desenvolvedores do projeto, mas também utilizados pelos clientes como documentação do trabalho. 


## Modelo Conceitual
Este é o modelo de mais alto nível, ou seja, que está mais próximo dos usuários.
O nível conceitual é desenvolvido com alto nível de abstração, a partir dos requisitos do sistema, extraídos da fase de levantamento de requisitos pelos analista de sistemas. 
Esse modelo pode ser elaborado de forma textual ou por meio de dois diagramas: Diagrama de Entidade e Relacionamento e/ou Diagrama de Classes

1) Clientes 
    Dados Necessários: Nome completo, endereço, bairro, cidade, etc ...
2) Pedido
    Dados Necessários: Código do produto, quantidade, código do cliente, etc ...

DER = Diagrama de Entidade e Relacionamento 
foto


## Modelo Lógico:
Este modelo descreve como os dados serão armazenados no banco de dados e também seus relacionamentos. Utilizando Banco de Dados Relacionais e Não Relacionais 

1) Forma de Representação: O tipo de dado que será armazenado em cada coluna com o nome de identificação da chave
foto

## Modelo Físico 
Também chamado de Modelo de Implementação, descreve, por meio de alguma linguagem, como será feita a armazenagem do banco. Nesse momento vamos identificar qual o Sistema utilizar.
foto

## Entidade (Tabela): 
Objeto ou evento do mundo real sobre o qual desejamos manter resitros em um banco de dados
- Entidade Produto
- Entidade Tipo de Produto

## Atributo Chave: 
Também conhecido como chave primária, Primary Key (PK), é um campo que deve possuir valor único em todo conjunto de dados da entidade. Este atributo é usado para identificar unicamente um registro de tabela 
- Entidade Produto: Código
- Entidade Tipo de Produto: Código 

## Relacionamentos: 
Geralmente as entidades nunca estõa sozinhas; normalmente estão assosicadas comoutras entidades. Reconhecer e registra os relacionamentos entre entidades fornece uma descrição muito mais rica do modelo. Um relacionamento pode acontecer entre uma, duas, várias entidades. 

## Chave Estrangeira:
Também conhecido como Foreign Key (FK), é um atributo presetnte em uma entidade que indica um relacionamento e representa a chave primária de uma outra entidade. 
- Entidade Produto: Código, cídigo do tipo de produto 
- Entidade Tipo de Produto: Código 

## Grau de Relacionamento 
Indica a quantidade de entidades ligadas a um relacionamento. Principais graus de relacionamento são: UNÁRIO, BINÁRIO E TERNÁRIO 

### UNÁRIO: uma entidade se relaciona com ela mesma. 
### BINÁRIO: uma entidade se relaciona com outra entidade. É o mais comum de relacionamento  
### TERNÁRIO: Três  entidade estão relacionadas por um mesmo relacionamento. 

## Credinalidade (Máxima): 
Define a quantidade máxima de ocorrênicas de uma entidade que poderá estar associada a outra entidade.
1) Relacionamento Binário Um-para-Um (1:1) (One-One)
  - Indida que uma ocorrênica da entidade A pode se relacionar exclusivamente com uma ocorrência da entidade B e vice versa. 
2) Relacionamento Binário Um-para-muitos(1:n)
  - Indica que uma ocorrência da entidade A pode se relacionar com várias ocorrências da entidade B, porém o inverso não é permitido. 
3) Relacionamento Binário Muitos-para-Muitos (n:m)
  - Indica que uma ocorrênica da entidade A pode se relacionar com várias ocorrências da entidade B e vice versa. 


# Normalização de Dados
Chamados de normalização de dados o processo formal e passo a passo que examina o documento descritivo gerado pelos analistas de sistemas durante a análise de requisistos em busca de definir as entidades, atributos, relacionamentos, chaves primárias e chaves estrangeiras de banco de dados a ser modelado. 

Este processo é realizado utilizando regras bem estabelecidas conhecidas como Formas Normais definadas por Edgar Frank Codd em seu artigo. 

Um dos objetivos principais da normalização é evitar ou pelo menos amenizar anomalias e inconsisttênicas que podem ocorrer furante a inclusão, exclusão, alteração e consulta de registros em um banco de dados.

Um banco de dados normalizado dentro dos padrões reduz o trabalho de manutenção e ajuda a evitar o desperdício do espaço de armazenamento, dentre outros benefícios.


## Primeira Forma Normal





























