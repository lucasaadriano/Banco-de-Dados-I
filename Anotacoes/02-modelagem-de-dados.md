# Modelagem de Dados

## 1. O que é modelagem de dados?

A modelagem de dados é o processo de representar e organizar os dados que um sistema precisa armazenar. Ela permite planejar quais informações serão necessárias, como serão estruturadas e quais relações existirão entre elas.

Antes de criar um banco de dados, é importante compreender o problema que precisa ser resolvido. A modelagem ajuda a transformar as necessidades de um sistema em uma estrutura organizada de dados.

## 2. Por que a modelagem é importante?

Uma modelagem bem planejada facilita a construção e a manutenção de um banco de dados. Quando as informações são organizadas de maneira inadequada, podem surgir problemas como dados duplicados, inconsistências e dificuldades para realizar consultas.

A modelagem ajuda a:

- Identificar os dados necessários para o sistema.
- Organizar as informações.
- Estabelecer relações entre os dados.
- Evitar redundâncias desnecessárias.
- Facilitar a implementação e a manutenção do banco de dados.

## 3. Exemplo prático

Imagine que uma faculdade precisa desenvolver um sistema para registrar seus alunos e as disciplinas em que estão matriculados.

Antes de criar o banco de dados, é necessário identificar as informações que precisam ser armazenadas.

**Aluno:**
- Código do aluno.
- Nome.
- E-mail.

**Disciplina:**
- Código da disciplina.
- Nome.
- Carga horária.

**Matrícula:**
- Código do aluno.
- Código da disciplina.
- Data da matrícula.

A modelagem permite perceber que alunos e disciplinas precisam ser relacionados por meio das matrículas.

## 4. Entidades e atributos

Na modelagem de dados, dois conceitos importantes são entidades e atributos.

**Entidade:** representa algo sobre o qual o sistema precisa armazenar dados. Pode ser uma pessoa, um objeto, um lugar ou um conceito.

Exemplos: Aluno, Professor, Disciplina e Produto.

**Atributo:** representa uma característica de uma entidade.

Por exemplo, a entidade Aluno pode possuir os atributos matrícula, nome, e-mail e data de nascimento.

## 5. Relacionamentos

Os relacionamentos representam as associações entre entidades.

Em uma faculdade, por exemplo, um aluno pode estar matriculado em várias disciplinas, enquanto uma disciplina pode ter vários alunos matriculados.

Esse tipo de associação é conhecido como relacionamento muitos para muitos (N:N).

Outras cardinalidades comuns são:

- **Um para um (1:1):** cada elemento de uma entidade está associado a, no máximo, um elemento da outra.
- **Um para muitos (1:N):** um elemento pode estar associado a vários elementos da outra entidade.
- **Muitos para muitos (N:N):** vários elementos de uma entidade podem estar associados a vários elementos da outra.

## 6. Níveis de modelagem

A modelagem de dados pode ser estudada em diferentes níveis:

- **Modelo conceitual:** apresenta uma visão geral dos dados e de seus relacionamentos, sem se preocupar com detalhes específicos de implementação.
- **Modelo lógico:** detalha a estrutura dos dados, incluindo tabelas, atributos, chaves e relacionamentos, de acordo com o modelo de banco de dados escolhido.
- **Modelo físico:** considera como os dados serão efetivamente implementados no SGBD, incluindo aspectos específicos de armazenamento e desempenho.

## Conclusão

A modelagem de dados permite planejar a estrutura de um banco de dados antes de sua implementação. Ao identificar entidades, atributos e relacionamentos, é possível representar as necessidades do sistema de maneira organizada e preparar sua estrutura lógica.
