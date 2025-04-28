# 📚 JoinMeInSQL 
**Repositório de anotações sobre SQL** | Um caderno digital com conceitos, exemplos práticos e exercícios para dominar Structured Query Language.  

![Badge](https://img.shields.io/badge/SQL-Study%20Notes-blue) 
![Badge](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)  

---

## 🏗️ Estrutura do Repositório  
```
sql-study-notes/ 
├── 1-Basics/ # Fundamentos do SQL 
├── 2-Intermediate/ # Tópicos intermediários 
├── 3-Advanced/ # Conceitos avançados 
├── 4-Examples/ # Projetos práticos 
├── 5-Cheatsheets/ # Resumos rápidos 
└── 6-Exercises/ # Desafios para praticar
```
## 🎲 Mas antes, o que são dados?
Dados são como pequenos pedaços de informção bruta que, sozinhos, podem parecer simples - como um número, uma palavra ou uma data. Mas quando organizados e analisados, eles contam histórias, revelam padrões e ajudam a tomar decisões inteligentes.  
Pensa assim:  
Um dado sozinho é uma peça de Lego. Sozinha, é só uma pecinha colorida.  
Muitos dados organizados viram uma estrutura! E ai sim, você constrói conhecimento, descobre tendências, cria relatórios ou até alimenta algoritmos de inteligência artificial.

## 🏦 E o que é um banco de dados?
Um banco de dados é como uma caixa mágica 📦 que guarda todos esses dados de forma estruturada. Imagina um super arquivo digital, ondo você pode guardar listas de clientes, produtos, notas, usuários ... tudo separadinho em tabelas, como se fossem planilhas! 📊  
Exemplo de uma tabela de clientes:
| ID          | Nome        | Email       |
|-------------|-------------|-------------|
| 1           | Ana Lima    | ana@email.com |
| 2 | João Reis | joao@email.com |


## 💻 E onde entra o SQL?
SQL (Structured Query Language) é a linguagem que usamos para conversar com os bancos de dados!  
Com o SQL você pode:
- 🔍 Buscar informações
- ➕ Adicionar novos dados
- 🛠️ Atualizar dados
- ❌ Deletar o que não precisa mais

Em resumo,  
- 🧠 Dados são informação
- 🏦 Banco de dados é onde essa informação mora
- 💬 SQL é a linguagem que você usa para interagir, organizar e manipular essas informações


## Diferença entre SQL, MySQL, PostgreSQL e Oracle Database
No mundo dos bancos de dados, nomes como MySQL, PostgreSQL e Oracle aparecem o tempo todo. Mas o que será que muda de um para o outro?


| Termo            | O que é?                            | Exemplo de Uso                                                  |
|------------------|-------------------------------------|-----------------------------------------------------------------|
| **SQL**          | Linguagem.                          | "Como" falamos com um banco de dados (ex: `SELECT * FROM tabela;`) |
| **MySQL**        | Sistema de banco de dados.          | Programa que armazena dados e entende SQL. Muito usado em sites e aplicações web. |
| **PostgreSQL**   | Sistema de banco de dados.          | Focado em ser robusto e confiável, ideal para projetos complexos. |
| **Oracle Database** | Banco de dados comercial (pago). | Usado por grandes empresas que precisam de alta performance e suporte oficial. |

## 🎯 Em resumo:

- **SQL** → É a **linguagem** 📖. (Assim como "Inglês" é uma língua, SQL é a língua dos bancos de dados.)
- **MySQL, PostgreSQL e Oracle** → São **programas** (bancos de dados) que **usam SQL** para se comunicar!


## 📊 Comparativo entre MySQL, PostgreSQL e Oracle

| Característica        | 🐬 MySQL                  | 🐘 PostgreSQL               | 🏛️ Oracle Database             |
|------------------------|----------------------------|------------------------------|---------------------------------|
| Licença                | Open Source (GPL)          | Open Source (PostgreSQL License) | Comercial (pago)               |
| Facilidade de uso      | Muito fácil de começar     | Fácil, mas mais técnico      | Exige conhecimento técnico     |
| Recursos avançados     | Bons, mas limitados        | Muito avançados              | Extremamente avançados         |
| Performance            | Excelente para leituras rápidas | Excelente para leitura e escrita | Altíssima em grandes volumes  |
| Suporte oficial        | Comunidade e Oracle (MySQL Enterprise) | Comunidade ativa            | Suporte premium da Oracle       |
| Ideal para             | Web Apps, Blogs, E-commerce | Sistemas robustos, bancos financeiros | Empresas grandes e críticas  |
| Exemplos de uso        | WordPress, Facebook        | Instagram, Spotify          | Bancos, Telecom, Governo        |

## 🎯 Resumo:

- **🐬 MySQL** → Ideal para projetos web que precisam ser simples e rápidos.
- **🐘 PostgreSQL** → Perfeito para aplicações mais robustas que exigem integridade e muitos recursos.
- **🏛️ Oracle Database** → Feito para grandes corporações que precisam de performance, suporte e segurança de alto nível.
--- 

## 📌 Conteúdo Detalhado  

### 1️⃣ **Fundamentos (Basics)**  
- [📌 Sintaxe básica](#-sintaxe-básica-select-insert-update-delete) (`SELECT`, `INSERT`, `UPDATE`, `DELETE`)  
- [🔍 Filtros](#-filtros-where-order-by-group-by) (`WHERE`, `ORDER BY`, `GROUP BY`)  
- [🔗 Junções](#-junções-inner-join-left-join-etc) (`INNER JOIN`, `LEFT JOIN`, etc.)  

### 2️⃣ **Intermediário (Intermediate)**  
- Subconsultas (subqueries)  
- Funções agregadas (`COUNT`, `SUM`, `AVG`)  
- Views e índices  

### 3️⃣ **Avançado (Advanced)**  
- Funções de janela (Window Functions)  
- Otimização de queries  
- Transações e ACID  

### 4️⃣ **Exemplos Práticos**  
- [Sistema de E-commerce](4-Examples/Ecommerce-DB/)  
- [Banco de dados para escola](4-Examples/School-DB/)  

### 5️⃣ **Cheatsheets**  
- [Comandos essenciais](5-Cheatsheets/SQL-Syntax.md)  
- [Diferenças entre SGBDs](5-Cheatsheets/PostgreSQL-vs-MySQL.md)  

### 6️⃣ **Exercícios**  
- [Nível iniciante](6-Exercises/Beginner/)  
- [Nível avançado](6-Exercises/Advanced/)  

---




---

### 📌 Sintaxe básica (`SELECT`, `INSERT`, `UPDATE`, `DELETE`)

Esses são os blocos de construção do SQL, usados para interagir com os dados:

```sql
-- SELECT: busca dados
SELECT * FROM produtos;

-- INSERT: insere dados
INSERT INTO produtos (nome, preco) VALUES ('Camiseta', 49.90);

-- UPDATE: atualiza dados existentes
UPDATE produtos SET preco = 59.90 WHERE id = 1;

-- DELETE: remove dados
DELETE FROM produtos WHERE id = 2;
```

### 🔍 Filtros (`WHERE`, `ORDER BY`, `GROUP BY`)
Filtros ajudam a encontrar exatamente o que você precisa nos dados.
``` sql
-- WHERE: filtra registros
SELECT * FROM clientes WHERE cidade = 'São Paulo';

-- ORDER BY: ordena os dados
SELECT * FROM produtos ORDER BY preco DESC;

-- GROUP BY: agrupa dados com base em uma coluna
SELECT categoria, COUNT(*) FROM produtos GROUP BY categoria;
```
### 🔗 Junções ('WINNER JOIN', 'LEFT JOIN', etc).
Junções são usadas para combinar dados de tabelas diferentes.
```sql
-- INNER JOIN: mostra apenas registros com correspondência nas duas tabelas
SELECT pedidos.id, clientes.nome
FROM pedidos
INNER JOIN clientes ON pedidos.cliente_id = clientes.id;

-- LEFT JOIN: mostra todos os registros da tabela da esquerda, mesmo sem correspondência
SELECT produtos.nome, categorias.nome AS categoria
FROM produtos
LEFT JOIN categorias ON produtos.categoria_id = categorias.id;
``` 

## 🔍 O que é uma operação de varredura simples (Full Table Scan)?
Uma operação de varredura simples (também chamada de full table scan) acontece quando o banco de dados varre linha por linha de uma tabela inteira, sem usar nenhum índice para filtrar ou localizar os dados.
## 📦 Como funciona:

--Imagine que você tem a tabela:

Clientes(id, nome, cidade, idade)

E você faz:
``` sql
SELECT nome FROM Clientes WHERE cidade = 'Belo Horizonte';
``` 
Se não houver índice sobre a coluna cidade, o banco de dados:

1. Vai pegar a tabela do início;
2. Ler todas as linhas, uma por uma;
3. Testar a condição cidade = 'Belo Horizonte';
4. E só então mostrar os nomes que satisfazem a condição.

## 🔥 Problemas de uma varredura completa:
🐢 Mais lenta em tabelas grandes
💾 Gasta muito I/O (leitura de disco)
🧠 Usa mais CPU
😩 Pode afetar o desempenho do sistema em consultas frequentes

## ✅ Quando ela pode ser aceitável?
- A tabela é pequena (poucas linhas)
- Você quer todos os dados da tabela
- A condição do WHERE retorna muitos registros (índice não vale a pena)
- Ainda não existem índices criados na coluna filtrada

## 🏗️ Como o otimizador decide?
O SGBD analisa:
- Tamanho da tabela
- Se há índice na coluna consultada
- Estatísticas de seletividade
- Custo estimado das opções

Se for mais “barato” fazer a leitura inteira do que seguir um índice mal seletivo, ele faz a varredura.


## 🛠️ Como Usar Este Repositório  

1. **Clone o projeto**:  
   ```bash
   git clone https://github.com/Isaisabelabela/JoinMeInSQL


## ✨ Créditos
Criado por Isabela com ❤️ e SELECT * FROM conhecimento

