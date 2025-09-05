# Procedure: INSERIR_FILM_ESTOQUE

Este script cria uma **stored procedure** no banco de dados `sakila` (MySQL).  
O objetivo é inserir no estoque (`inventory`) os filmes que ainda não possuem cópias cadastradas.

## 📋 Parâmetros
- `CODIGO_STORE (INT)` → código da loja onde os filmes serão inseridos no estoque.  
- `ULTIMO_NUMERO_MATRICULA (INT)` → quantidade de cópias (itens de inventário) que devem ser adicionadas para cada filme.

## ⚙️ Como usar
1. Certifique-se de estar no banco `sakila`:
   ```sql
   USE sakila;
2. Crie a procedure executando o script:
 ```
   DELIMITER $
CREATE PROCEDURE INSERIR_FILM_ESTOQUE(IN CODIGO_STORE INT, IN ULTIMO_NUMERO_MATRICULA INT)
BEGIN
    -- código da procedure
END$
DELIMITER ;
```
3. Chame a procedure informando os parâmetros desejados:
  ```
CALL INSERIR_FILM_ESTOQUE(1, 5);
```
