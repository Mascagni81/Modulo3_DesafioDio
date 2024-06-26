# Desafio Módulo 3 – Processamento de Dados Simplificado com Power BI

## Descrição:
### 1. Criação de uma instância na Azure para MySQL

### 2. Criar o Banco de Dados com base disponível no GitHub

### 3. Integração do Power BI com MySQL no Azure

### 4. Verificar problemas na base a fim de realizar a transformação dos dados


## Diretrizes para transformação dos dados:
### 1. Verifique os cabeçalhos e tipos de dados

### 2. Modifique os valores monetários para o tipo double preciso

### 3. Verifique a existência dos nulos e analise a remoção

### 4. Os employees com nulos em `Super_ssn` podem ser os gerentes. Verifique se há algum colaborador sem gerente

### 5. Verifique se há algum departamento sem gerente

### 6. Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas

### 7. Verifique o número de horas dos projetos

### 8. Separar colunas complexas

### 9. Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção

### 10. Neste processo elimine as colunas desnecessárias.

### 11. Realize a junção dos colaboradores e respectivos nomes dos gerentes. Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.

- Foi utilizado a tabela `employee_depart` para realizar a mesclagem de `SSN` com `Super_SSN` da tabela `employee`, onde o campo `FName` foi atualizado como `Manager`.

### 12. Mesclar as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores

### 13. Mesclar os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.

### 14. Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir.

- As tabelas foram mescladas porque são complementares entre si, onde podemos acrescentar as colunas de uma em outra. No entanto, se houvesse dados iguais, poderia ser utilizado o recurso acrescentar.

### 15. Agrupe os dados a fim de saber quantos colaboradores existem por gerente

### 16. Elimine as colunas desnecessárias, que não serão usadas no relatório, de cada tabela


### Power BI
<img src="./imgs/img1.PNG">
<img src="./imgs/img2.PNG">
<img src="./imgs/img3.PNG">

