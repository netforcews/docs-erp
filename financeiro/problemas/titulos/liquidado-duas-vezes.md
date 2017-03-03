# Título liquidado duas vezes

## Problema/Situação
Você emitiou um boleto de cobrança para seu cliente e depois de uns dias quando foi verificar o histórico dessa cobrança se deparou com
duas ocorrências de liquidação quando na verdade deveria existir somente uma:

![ocorrencias](https://raw.githubusercontent.com/netforcews/docs-erp/master/financeiro/imagens/ocorrencias.png)
> Nota que a primeira ocorrência é a "06" e a segunda "17"

## Causas

1. O cliente pode ter se enganado e pagado o mesmo boleto duas vezes.
Vamos supor que temos um título com 3 parcelas, 1234/A, 1234/B e 1234/C. O cliente pagou a parcela 1234/A, e quando foi para pagar a
parcela 1234/B acidentalmente pagou a 1234/A novamente.
Você irá receber o arquivo de retorno do banco duas vezes, e quando importar no sistema você vai reparar que a mesma parcela do 
título possuí 2 liquidações, provavelmente cada uma das liquidações com ocorrências diferentes.


## Solução
Para resolver esse impasse você precisa verificar no Banco se realmente o dinheiro entrou duas vezes, se sim, você precisará dar baixa
no título 1234/B afinal ele teoricamente já foi pago, importar o arquivo de retorno do Banco no sistema e por fim fazer o pagamento 
da parcela 1234/B manualmente no sistema.
