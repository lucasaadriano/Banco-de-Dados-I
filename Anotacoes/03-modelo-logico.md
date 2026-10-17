# Modelo Lógico de Banco de Dados

## 1. O que é o modelo lógico?

O modelo lógico é uma representação estruturada dos dados que define como as informações serão organizadas no banco de dados. No modelo relacional, essa estrutura é representada principalmente por tabelas, colunas, chaves e relacionamentos.

Ele faz a ligação entre a modelagem conceitual, que representa as necessidades do sistema, e a implementação do banco de dados.

## 2. Tabelas, colunas e registros

No modelo relacional, os dados são organizados em tabelas.

Uma tabela é formada por colunas e registros, também chamados de linhas.

- **Tabela:** reúne dados de uma determinada categoria.
- **Coluna:** representa um atributo, como nome, e-mail ou data de nascimento.
- **Registro:** representa um conjunto de valores correspondentes a um elemento cadastrado.

Por exemplo, uma tabela chamada Aluno poderia ser representada assim:

| id_aluno | nome | email |
|---:|---|---|
| 1 | Ana | ana@email.com |
| 2 | Pedro | pedro@email.com |
| 3 | Maria | maria@email.com |

Nesse exemplo, `Aluno` é a tabela, `nome` é uma coluna e cada linha representa um registro de aluno.

## 3. Chave primária

A chave primária, ou *Primary Key (PK)*, é um atributo ou conjunto de atributos utilizado para identificar cada registro de maneira única dentro de uma tabela.

Na tabela Aluno, o atributo `id_aluno` pode ser utilizado como chave primária, pois cada aluno possui um identificador próprio.

A chave primária não deve se repetir e não pode receber valor nulo.

## 4. Chave estrangeira

A chave estrangeira, ou *Foreign Key (FK)*, é um atributo utilizado para estabelecer uma relação entre tabelas.

Imagine duas tabelas:

**Aluno**

| id_aluno (PK) | nome |
|---:|---|
| 1 | Ana |
| 2 | Pedro |

**Matricula**

| id_matricula (PK) | id_aluno (FK) | disciplina |
|---:|---:|---|
| 101 | 1 | Banco de Dados |
| 102 | 2 | Matemática |
| 103 | 1 | Programação |

A coluna `id_aluno` da tabela Matricula é uma chave estrangeira que referencia a tabela Aluno. Dessa forma, é possível identificar qual aluno está associado a cada matrícula.

## 5. Relacionamentos entre tabelas

Os relacionamentos permitem associar informações armazenadas em tabelas diferentes.

No exemplo anterior, um aluno pode possuir várias matrículas. Esse relacionamento é do tipo um para muitos (1:N).

Quando existe um relacionamento muitos para muitos (N:N), geralmente é necessário criar uma tabela intermediária para representar as associações.

Por exemplo, alunos podem cursar várias disciplinas, e cada disciplina pode ter vários alunos. Uma tabela Matrícula pode representar essa relação.

## 6. Tipos de dados

Cada coluna de uma tabela possui um tipo de dado, que determina quais valores podem ser armazenados nela.

Alguns exemplos comuns são:

- `INTEGER`: números inteiros.
- `VARCHAR`: textos com tamanho variável.
- `DATE`: datas.
- `DECIMAL`: números com casas decimais.

A escolha do tipo de dado deve considerar a informação que será armazenada e as regras do sistema.

## 7. Restrições de integridade

As restrições de integridade ajudam a manter os dados corretos e consistentes.

Alguns exemplos são:

- **PRIMARY KEY:** identifica cada registro de forma única.
- **FOREIGN KEY:** mantém a relação entre tabelas.
- **NOT NULL:** impede que uma coluna receba valor nulo.
- **UNIQUE:** impede valores duplicados na coluna ou conjunto de colunas definido.

Essas regras ajudam a evitar informações inválidas e relacionamentos inconsistentes.

## Conclusão

O modelo lógico define como os dados serão organizados e relacionados. No modelo relacional, compreender tabelas, colunas, registros, chaves, relacionamentos e tipos de dados é essencial para construir bancos de dados estruturados e consistentes.
