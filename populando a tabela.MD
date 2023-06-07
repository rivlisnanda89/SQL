-- insering data of the table

INSERT INTO nome_da_tabela (nome_da_coluna1, nome_da_coluna2, ...) VALUES (valor_a_ser_inserido_na_coluna1, valor_a_ser_inserido_na_coluna2, ...)

Depois de inseridos, é possível que os dados sofram alteração de acordo com a dinâmica do negócio ou do projeto a que os dados se referem. Por exemplo, clientes podem mudar de endereço e saldos mudam em contas-correntes. Para fazer estas alterações, o SQL possui o comando UPDATE, que tem a sintaxe a seguir:


UPDATE nome_da_tabela SET nome_da_coluna = novo_valor_do_dado_da_coluna WHERE condições

Da mesma forma, é possível que determinado dado, não mais necessário ou inserido por engano, seja excluído da tabela. Um produto incluído indevidamente no banco de dados precisa ser retirado. Para isso, utiliza-se o comando DELETE, que é escrito desta maneira:


DELETE FROM nome_da_tabela WHERE condições
