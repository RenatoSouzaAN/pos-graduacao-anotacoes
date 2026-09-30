𝗗𝗤𝗟 (𝗗𝗮𝘁𝗮 𝗤𝘂𝗲𝗿𝘆 𝗟𝗮𝗻𝗴𝘂𝗮𝗴𝗲):  
O que faz: Consulta os dados no banco de dados.  
Comandos comuns: SELECT.  
Exemplo: SELECT * FROM employees WHERE position = 'Developer';  
  
𝗗𝗠𝗟 (𝗗𝗮𝘁𝗮 𝗠𝗮𝗻𝗶𝗽𝘂𝗹𝗮𝘁𝗶𝗼𝗻 𝗟𝗮𝗻𝗴𝘂𝗮𝗴𝗲):  
O que faz: Manipula os dados dentro das tabelas.  
Comandos comuns: SELECT, INSERT, UPDATE, DELETE.  
Exemplo: INSERT INTO employees (name, position) VALUES ('Ana', 'Developer');  
  
𝗗𝗗𝗟 (𝗗𝗮𝘁𝗮 𝗗𝗲𝗳𝗶𝗻𝗶𝘁𝗶𝗼𝗻 𝗟𝗮𝗻𝗴𝘂𝗮𝗴𝗲):  
O que faz: Define a estrutura do banco de dados.  
Comandos comuns: CREATE, ALTER, DROP, TRUNCATE.  
Exemplo: CREATE TABLE employees (id INT PRIMARY KEY, name VARCHAR(50), position VARCHAR(50));  
  
𝗗𝗖𝗟 (𝗗𝗮𝘁𝗮 𝗖𝗼𝗻𝘁𝗿𝗼𝗹 𝗟𝗮𝗻𝗴𝘂𝗮𝗴𝗲):  
O que faz: Controla o acesso aos dados.  
Comandos comuns: GRANT, REVOKE.  
Exemplo: GRANT SELECT ON employees TO user_name;  
  
𝗗𝗧𝗟 (𝗗𝗮𝘁𝗮 𝗧𝗿𝗮𝗻𝘀𝗮𝗰𝘁𝗶𝗼𝗻 𝗟𝗮𝗻𝗴𝘂𝗮𝗴𝗲):  
O que faz: Gerencia o fluxo de transações de dados.  
Comandos comuns: BEGIN TRANSACTION, END TRANSACTION.  
Exemplo: BEGIN TRANSACTION; INSERT INTO employees (name, position) VALUES ('Ana', 'Developer'); COMMIT;  
  
  
Fonte da imagem: Blog da Trybe

![[1716814889101.jpg]]
