
# Resolução exercício SQL

Atividade SQL passada pelo professor adison em sala para terminar em casa


## 1ª Questão
Selecione todos os dados dos países da tabela_paises;

```sql
select*from tabela_paises
```
## Resultado esperado

![q1](https://github.com/FlavioJuniorhr/SQL/assets/111861420/b5cf21c9-73b5-4521-816d-38708a4e25f0)



## 2ª Questão
Selecione todas as cidades cujo país seja brazil;

```sql
select cidade from tabela_paises where pais = 'Brazil
```
## Resultado esperado

![q2](https://github.com/FlavioJuniorhr/SQL/assets/111861420/79c1aa19-d590-4535-88d5-a5f6ef670f68)


## 3ª Questão
Selecione todas as cidades cuja região(estado) é ceará;
```sql
select cidade from tabela_paises where regiao = 'Ceará'
```
## Resultado esperado

![q3](https://github.com/FlavioJuniorhr/SQL/assets/111861420/69686404-5376-47f7-b47b-0a77da865738)

## 4ª Questão
Utilize a função count para saber quantas regiões(estados) existem na China,
utilize também o group by;

```sql
select count(regiao) from tabela_paises where pais = 'China' group by regiao
```
## Resultado esperado

![q4](https://github.com/FlavioJuniorhr/SQL/assets/111861420/43fc3931-2d79-4d8a-9cb1-aae1d363262f)


## 5ª Questão
Quais regiões, diferentes, existem no Canadá?

```sql
select count(distinct regiao) from tabela_paises where pais = 'Canada'
```
## Resultado esperado

![q5](https://github.com/FlavioJuniorhr/SQL/assets/111861420/d6414c8c-e862-493c-9226-65ac271ff5b6)


## 6ª Questão
Quantos países diferentes existem na tabela 'tabela_paises';

```sql
select distinct pais from tabela_paises
```
## Resultado esperado

![q6](https://github.com/FlavioJuniorhr/SQL/assets/111861420/4ba297b4-ba6b-4f9a-b9bb-9f1fdd6b8099)


## 7ª Questão
Quantas cidades diferentes existem no brazil;

```sql
select distinct cidade from tabela_paises where pais = 'Brazil'
```
## Resultado esperado

![q7](https://github.com/FlavioJuniorhr/SQL/assets/111861420/34a728d1-d748-440d-9b4d-c99b46be571e)


## 8ª Questão
Selecione os países e quantas regiões cada país possui;

```sql
select pais,count(regiao) from tabela_paises group by pais
```
## Resultado esperado

![q8](https://github.com/FlavioJuniorhr/SQL/assets/111861420/c7fe97ee-4cfe-44ba-b4c5-50eaefb58a1d)



## 9ª Questão
Quantas pessoas com nome começando em 'João' existem no banco?

```sql
select count(nome) from tabela_paises where nome like 'João%'
```
## Resultado esperado

![q9](https://github.com/FlavioJuniorhr/SQL/assets/111861420/10e779d5-5e8c-48f0-9b07-5706eb6654e9)


## 10ª Questão
Quantas pessoas têm o nome John?

```sql
select count(nome) from tabela_paises where nome = 'John'
```
## Resultado esperado

![q10](https://github.com/FlavioJuniorhr/SQL/assets/111861420/0709ae8d-4093-4428-9564-c6a5603e2a19)


## 11ª Questão
Ordene os nomes dos países sem repetição em ordem alfabética;

```sql
select distinct pais from tabela_paises order by pais ASC
```
## Resultado esperado

![q11](https://github.com/FlavioJuniorhr/SQL/assets/111861420/773f28cb-5644-46a1-8529-0908baafb393)
