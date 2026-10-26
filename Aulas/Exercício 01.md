CREATE DATABASE db_clubepaysandu;
USE db_clubepaysandu;

CREATE TABLE tb_socio (
codS INTEGER auto_increment NOT NULL,
nomeS VARCHAR(50) NOT NULL,
sexoS ENUM('FEMININO','MASCULINO','OUTROS'),  
data_nascS DATE,
primary key (codS)
)

CREATE TABLE tb_dependente(
ID INTEGER NOT NULL,
nomeDep VARCHAR(50) NOT NULL,
codS INTEGER,
primary key (ID),

/*ALTERANDO NOME E TAMANHO LIMITE DE 50 PARA 100 */

ALTER TABLE tb_socio  CHANGE nomeS nomeSocio VARCHAR(100) NOT NULL

/* ADICIONANDO VARIÁVEIS */

ALTER TABLE tb_socio ADD CPF VARCHAR (14)

ALTER TABLE tb_socio ADD fone VARCHAR (14)

/*criar uma nova tabela!*/

DROP TABLE tb_dependente;

CREATE TABLE tb_dependente (
ID INTEGER NOT NULL,
nomeDep VARCHAR(30) NOT NULL,
codS INTEGER
)

ALTER TABLE tb_dependente ADD PRIMARY KEY (ID)

ALTER TABLE tb_dependente ADD FOREIGN KEY (codS) references tb_socio (codS)PRIMARY
