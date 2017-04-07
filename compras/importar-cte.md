# Importação de CT-e

Conhecimento de Transporte Eletrônico (CT-e) é um documento fiscal brasileiro emitido pelas transportadoras de carga para 
cobrir as mercadorias entre a localidade de origem e o destinatário da carga. Para a própria empresa transportadora, esse documento 
é a sua nota fiscal, ou seja, é o documento oficial usado para contabilizar as receitas e efetivar o faturamento.


## Importar XML

Para fazer a importação de uma CT-e no *Sistema NetForce* siga os seguintes passos:

1. Entre no módulo ```Compras``` e em seguida clique na opção do menu lateral esquerdo ```Importar CT-e```:

![importar](https://raw.githubusercontent.com/netforcews/docs-erp/master/compras/imgs/importar.png)

2. Em seguida clique no comando **Importar CT-e** e na tela que se abre procure e selecione o XML da CT-e em **Escolher Arquivo**. Por fim,
clique em **Anexar**:

![selecionar-xml](https://raw.githubusercontent.com/netforcews/docs-erp/master/compras/imgs/selecionar-xml.png)

3. Depois de realizar esses passos e caso tudo der certo, você retornará para o grid e a mensagem 
em verde ```XML do CT-e importado com sucesso!``` irá aparecer.
Caso der algum erro, procure por ele na sessão de **Erros** nesse mesmo manual que você está lendo.

![sucesso](https://raw.githubusercontent.com/netforcews/docs-erp/master/compras/imgs/sucesso.png)

## Visualizando a CT-e

![interface](https://raw.githubusercontent.com/netforcews/docs-erp/master/compras/imgs/interface.png)

### Geral

Campo |
------|
**Tipo de CTe**
**Tipo de Serviço**
**Emissão**
**Munícipio de Origem**
**Número**
**Série**
**CFOP**
**CT-e XML**
```Remetente``` |
**Município Início**
**Estado Início**
```Destinatário``` |
**Município Fim**
**Estado Fim**
```Componentes do Frete``` |
**Valor do Frete**
**Modal**
```Mercadoria``` |
**Outras características da carga**
**Produto Predominante**
**Valor Total de Tributos**
**Valor a Receber**
**Valor Total de Carga**
```Fisco``` |
**Info.Adicional**

### Componentes

Campo |
------|
**Nome**
**Valor**

### Mercadorias

Campo |
------|
**Unidade**
**Tipo de Medida**
**Quantidade de Carga**
**Valor da Carga para Averbação**

### Documentos

Campo |
------|
**Chave**
**NF-e ou Doc. Anterior**

### Impostos

Campo |
------|
**Tipo CST**
**Número CST**
**Descrição CST**
**Valor BC**
**% ICMS**
**Valor ICMS**
**% Redução BC**
**Valor BC do ICMS ST retido**
**Valor ICMS ST Retido**
**% ICMS ST Retido**
**Valor Crédito**
**Simples Nacional**
**% ICMS FCP**
**Valor ICMS FCP**
**% ICMS Interestadual**
