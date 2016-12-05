# Devolução - Nota Fiscal

Para realizar a devolução de uma nota fiscal, siga os seguintes passos:

1. Primeiro acesse o módulo de ```Vendas``` do sistema:

![mod-vendas](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/mod-vendas.png)

2. Em seguida navegue para a opção ```Pedidos```:

![pedidos](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/pedidos.png)

3. Para efetuar a devolução da nota fiscal, você precisará criar um novo pedido com as mesmas informações do pedido que você quer fazer a devolução, a diferença será nos campos a seguir:

  ### Aba Geral
  1. ```Natureza de Operação```, terá que ser uma de devolução:
  
  ![natOp](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/natOp.png)
  
  2. ```Condição de Pagamento```, terá que ser **Simples Remessa**:
  
  ![cond-pag](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/cond-pag.png)
  
  3. ```Forma de Pagamento```, também terá que ser **Simples Remessa**:
  
  ![forma-pag](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/forma-pag.png)
  
  ### Aba NotaFiscal
  ![notaFiscal](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/notaFiscal.png)
  
  1. ```Finalidade```, necessita ter o conteúdo **Devolução**:
  
  ![finalidade](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/finalidade.png)
  
  2. ```Nota Referente```, neste campo você deve colocar os 44 caracteres que compõem a chave da nota fiscal que você está fazendo a 
  devolução:
  
  ![nota-referente](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/nota-referente.png)
  
> Lembrando que nos itens do pedido a **CFOP** terá que ser a mesma dos itens do pedido que você está fazendo a devolução.

Depois de ter concluído todos os passos basta salvar o pedido e lançar o mesmo como qualquer outro pedido:

![lancar](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/lancar.png)
