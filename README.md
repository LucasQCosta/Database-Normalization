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
