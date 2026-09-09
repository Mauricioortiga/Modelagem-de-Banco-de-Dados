Norma vem de normalização

Precisamos de regras para projetar um banco de dados

Estas regras de normalização, chamamos de:

1FN: Primeira Forma Normal

2FN: Segunda Forma Normal

3FN: Terceira Forma Normal

4FN: Quarta Forma Normal

Uma forma normal é uma regra que deve ser obedecida por uma tabela para que esta seja considerada "bem projetada".

O que precisamos entender:

Para fazer bons projetos, precisamos elaborar modelos conceituais, em cada projeto, determinamos os números de tabelas dependendo do que irá guardar, das regras aplicadas

Um bom projeto começa com uma tabela grande, sendo quebrada em duas, para analisar se é necessário quebrar novamente.

PROVA: **Elabore um modelo conceitual seguindo as formas de normalização:**

Significa normalizar uma tabela em até 3 tabelas.

Tabela não-normalizada = tabela que contém outras tabelas alinhadas (Uma tabela cheia de dados, claramente sendo uma tabela dentro da outra).

**Precisamos saber o que é um atributo Multivalorado.**

OLHAR ARQUIVO: 10a. NORMALIZACAO - com resposta cenário Biblioteca.pptx

COMO APLICAR AS FORMAS:

**1FN:** Uma tabela está na primeira forma normal, quando ELA NÃO CONTÉM TABELAS ALINHADAS.

1. Não quebrar e manter uma única tabela grande.

2. Construir uma tabela para cada tabela alinhada, não pode haver tabelas alinhadas.

Modelo textual:

Proj (CodProj, tipo, descr)

projEmp {codproj, codEmp, (DESLOCA PARA EMP PORQUE PERTENCE AO EMP= nome, cat, sal,) Dataini, TempAl)}

Emp (codemp, nome, cat, sal)

**2FN:** Uma tabela encontra-se na segunda forma normal, quando, além de estar na 1FN, mão contém dependências parciais.

1. Não pode haver dependência funcional parcial
Uma dependência funcional parcial ocorre quando uma coluna depende apenas de parte de uma chave primária composta

Se perceber que algum atributo está dependendo de alguma chave composta, você terá que dividir em duas.

Se algum atributo não depender de uma chave composta, terá que quebrar a tabela.


**3FN:** Uma tabela encontra-se na terceira forma normal, quando, além de estar na 2FN, não contém dependências transitivas.

**uma dependência funcional transitiva ocorre quando uma coluna, além de depender da chave primária da tabela, depende de outra coluna ou conjunto de colunas da tabela.**

FIXE AS REGRAS: SEMPRE A PARTIR DE UMA TABELA NÃO NORMALIZADA, SE PERGUNTE QUAIS SÃO AS FORMAS NOMINAIS A SEREM APLICADAS.

---

DDL - Linguagem de definição de dados:

CREATE
DROP
ALTER

---

Em esquemas, é a área onde se digita os comandos.

---

Em uma database para criar uma base de dados, selecione Esquemas, ao lado de Administração:

PRIMEIRO COMANDO:

Create database db_empresa_FeatHype; (Nome da empresa)
(Criando uma base de dados) / (Nome da empresa)

No raio amarelo, abaixo vai mostrar o DEBUG ou SAÍDA DE DADOS.

No canto esquerdo, precisamos dar Refresh all para aparecer a saída de dados.

SEGUNDO COMANDO:

Use db_empresa_FeatHype;

TERCEIRO COMANDO:

Create table tb_cliente (
codCLI (DÊ UM ESPAÇO E INFORME O TIPO DE DADO) integer (inteiro) not null (Não pode ser nulo) primary key (Chave Primária),
nomeCLI varchar(100) (String com 100 caracteres) not null (PRECISA COLOCAR PARA NÃO CADASTRAR UM USUÁRIO SEM NOME), 
Sexo char(1),
dt_niverCLI date (Não se coloca vírgula porque é o último)

)


