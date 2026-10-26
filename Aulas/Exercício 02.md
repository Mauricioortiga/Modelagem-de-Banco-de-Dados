CREATE DATABASE db_clinica_flor;
USE db_clinica_flor;

CREATE TABLE tb_medico(
CRM INTEGER NOT NULL PRIMARY KEY,
nomeM VARCHAR(100) NOT NULL
);

CREATE TABLE tb_paciente(
ID INTEGER NOT NULL PRIMARY KEY,
nomePAC VARCHAR(100) NOT NULL
);


CREATE TABLE tb_consulta(
CRM INTEGER NOT NULL,
ID INTEGER NOT NULL,
data_consulta DATE,
hora_consulta TIME,
PRIMARY KEY (CRM, ID),
FOREIGN KEY (CRM) references tb_medico (CRM),
FOREIGN KEY(ID) references tb_paciente(ID)
);

INSERT tb_medico VALUES (1010, 'JOSÉ MARIA');
INSERT tb_medico VALUES (1011, 'DIEGO');
INSERT tb_medico VALUES (1012, 'DIOGO');
INSERT tb_medico VALUES (1013, 'GABRIEL');

SELECT *
FROM tb_medico
WHERE CRM=1012

SELECT *
FROM tb_medico
WHERE nomeM='Gabriel'

INSERT tb_paciente VALUES (1, 'JOSYANE'), (2, 'MARCOS'), (3, 'ANA'), (4, 'MAITE')

SELECT nomePAC
FROM tb_paciente
ORDER BY nomePAC DESC ou ASC
