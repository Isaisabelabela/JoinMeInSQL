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

### 🔍 Filtros (`WHERE`, `ORDER BY`, `GROUP BY`)
Filtros ajudam a encontrar exatamente o que você precisa nos dados.
``` sql
-- WHERE: filtra registros
SELECT * FROM clientes WHERE cidade = 'São Paulo';

-- ORDER BY: ordena os dados
SELECT * FROM produtos ORDER BY preco DESC;

-- GROUP BY: agrupa dados com base em uma coluna
SELECT categoria, COUNT(*) FROM produtos GROUP BY categoria;


## 🛠️ Como Usar Este Repositório  

1. **Clone o projeto**:  
   ```bash
   git clone https://github.com/Isaisabelabela/JoinMeInSQL


## ✨ Créditos
Criado por Isabela com ❤️ e SELECT * FROM conhecimento

