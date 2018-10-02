# BOLETOS, COMO FUNCIONA?

Primeiramente vamos preciar entender alguns conceitos e processos.

## Remessa de cobrança
É um arquivo gerado pelo sistema para o banco, em layout definido pelo banco com informaçoes necessárias para registro e controle de títulos.

## Retorno de cobrança
É um arquivo gerado pelo banco para o sistema, em layout definido pelo banco com informações necessáiras para atualização e controle de de títulos enviados pelo sistema.

## Processo
1. A cada pedido fechado, que gerar uma Nota Fiscal, o sistema faz uma marcação de controle;
2. Após um período qualquer - pode ser a cada 2 horas, no fim do expediente, conforme critério da sua empresa - deve-se fazer a **Remessa de cobrança**.
Neste caso, o sistema irá gerar um arquivo de remessa apenas dos títulos marcados até o momento. Este arquivo deve ser enviado através do portal do banco;
3. Feito isto, geralmente 24 horas depois, deve-se acessar o portal do banco e baixar o arquivo de retorno, o **Retorno de cobrança**, para importar no sistema, que buscará consciliar as informações recebidas com as informações enviadas.

## Lembre-se
A forma de pagamento do título deve ser **Boleto**.
![boletoformapagamento](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/boletoformapagamento.png)
Dados do boleto
![boletodados](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/boletodados.png)
Para emitir o boleto, deve-se estar no título desejhado,e na parte inferior dos dados há uma opção **Boleto**
![boletoimprimir](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/boletoimprimir.png)
<br>

## Veja:
- [Remessa de Cobrança](/financeiro/contacobranca.md)
- [Retorno de Cobrança](/financeiro/cobranca.md)
- [Contas a Receber](/financeiro/contasareceber.md)

