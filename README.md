## Type of Normalization

### 1. First Normal Form (1FN)

Each attribute must contain only atomic values.

To address this, we created a new table to reference the phones based on employees, removing them from the Clients table.

Cada atributo deve conter apenas valores atômicos

Para resolver isso, criamos uma nova tabela para referênciar os telefones de acordo com os colaboradores. Retirando assim da tabela Clientes.

### 2. Second Normal Form (2FN)

Firstly, it needs to be in the first standard form. Furthermore, a table cannot contain partial dependencies (two primary keys).

To achieve this, we created a new table by splitting the Orders table into two: Orders and Order_Items, where one has the primary key as COD_PEDIDO (Pedidos) and the other has COD_PEDIDO and COD_LIVRO (Itens_pedidos) as primary keys.

Primeiramente, ela precisa estar na primeira forma normal. Além disso, uma tabela não pode conter dependências parciais (Duas chaves primárias).

Para isso, criamos uma nova tabela, dividindo a tabela Pedidos: Pedidos e Itens_Pedidos, em que uma tema como chave primária a chave COD_PEDIDO (Pedidos) e a outra tem COD_PEDIDO e COD_LIVRO (Itens_pedidos).

### 3. Third Normal Form (3FN)

Essas tabelas possuem depedência transitiva, que consiste em uma forma de dependência funcional indireta.

### 4. Third Normal Form Boyce Codd (3FN BC)

Quando depender de outro atributo não chave (chave candidata ou primária). Ou seja, uma tabela estará na BCNF se e somente se estiver na 3FN e todo atributo não chave depender funcionalmente diretamente da chave primária.

### 5. Fourth Normal Form Boyce Codd (4FN)

É focada em eliminar dependências multivariadas entre os atributos chave.  Isto é, se há mais atributos (além das chaves primárias ou estrangeiras) que se repetem na tabela. Se isso ocorrer, geramos novas tabelas para eliminar tal redundância e manter as relações entre os atributos.