# Importar CT-e

Conhecimento de Transporte Eletrônico (CT-e) é um documento fiscal brasileiro emitido pelas transportadoras de carga para 
cobrir as mercadorias entre a localidade de origem e o destinatário da carga. Para a própria empresa transportadora, esse documento 
é a sua nota fiscal, ou seja, é o documento oficial usado para contabilizar as receitas e efetivar o faturamento.


## Importar XML

Para fazer a importação de uma CT-e no *Sistema NetForce* siga os seguintes passos:

1. Entre no módulo ```Compras``` e em seguida clique na opção do menu lateral esquerdo ```Importar CT-e```:

![importar](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/importarcte01.png)

2. Em seguida clique no comando **Importar CT-e** e na tela que se abre procure e selecione o XML da CT-e em **Escolher Arquivo**. Por fim, clique em **Anexar**:

![selecionar-xml](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/importarcte02.png)
![selecionar-xml2](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/importarcte03.png)

3. Depois de realizar esses passos e caso tudo der certo, você retornará para o grid e a mensagem 
em verde ```XML do CT-e importado com sucesso!``` irá aparecer.
Caso der algum erro, procure por ele na sessão de **Erros** nesse mesmo manual que você está lendo.

![sucesso](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/importarcte04.png)

## Erros

### CT-e já foi importada

#### Problema
Você foi importar uma CT-e normalmente e recebeu esse erro.

#### Solução
Isso quer dizer que já existe a CT-e que você está tentando importar no sistema. Verifique se você selecionou o arquivo certo na hora
de anexar o mesmo.

### Notas de homologação não devem ser importadas

#### Problema
Caso você obtenha esse erro você está tentando importar um XML com o tipo de ambiente 2, referente a homologação.
No seu XML a tag **tpAmb** vai estar com o valor 2, para importar uma CT-e essa tag precisa ter o valor 1, referente a produção.

#### Solução
Nesse caso o seu XML não está apto para a importação, verifique com a transportadora e solicite um novo XML CT-e autorizado.

### O XML selecionado não é uma CT-e autorizada ou não é uma CT-e

#### Problema
Você escolheu seu arquivo e clicou no botão anexar e em seguida obteve esse erro retornando para o grid.

#### Solução
Como a mensagem diz, o XML selecionado não é uma CT-e ou é uma CT-e autorizada. Verifique o seu XML e tenha certeza se você está
selecionando o arquivo certo para realizar o anexo.

### Arquivo não foi transferido corretamente 

#### Problema
Você escolheu seu arquivo e clicou no botão anexar e em seguida obtém esse erro na mesma tela em que está.

#### Solução
Provavelmente você selecionou um arquivo que não se encaixa na importação do xml, ou seja, selecionou um arquivo que não possui
a extensão **.xml**. Tenha certeza que o seu arquivo possui a extensão **.xml**, verifique se você está pegando o arquivo correto e 
tente importar novamente.

### Arquivo "nomedoseuarquivo" do XML-CTe não foi encontrado

#### Problema
Esse erro pode ocorrer depois que você clicar no botão **Anexar** logo depois de ter escolhido o seu arquivo para importação.

#### Solução
Ocorreu algum conflito no sistema, apenas repita os procedimentos e tente anexar o arquivo novamente, caso ainda não obter sucesso contate o *Suporte NetForce*.

## Visualizando a CT-e

![interface](https://raw.githubusercontent.com/netforcews/docs-erp/master/faq/imagens/importarcte05.png)

### Geral

**Campo** | **Descrição**
----------|--------------
Tipo de CTe | Tipo do CT-e
Tipo de Serviço | Tipo do Serviço
Emissão | Data e hora de emissão do CT-e
Munícipio de Origem | Código do Município de envio do CT-e (de onde o documento foi transmitido) 
Número | Número do CT-e
Série | Série do CT-e 
CFOP | Código Fiscal de Operações e Prestações 
CT-e XML | XML do CT-e

**Remetente** | **Descrição**
--------------|--------------
Município Início | Município de início da prestação
Estado Início | Estado do início da prestação

**Destinatário** | **Descrição**
-----------------|--------------
Município Fim | Município de término da prestação 
Estado Fim | Estado do término da prestação

**Componentes do Frete** | **Descrição**
-------------------------|--------------
Valor do Frete | Valor Total da Prestação do Serviço 
Modal | Modal 

**Mercadoria** | **Descrição**
---------------|--------------
Outras características da carga | Outras características da carga 
Produto Predominante | Produto predominante 
Valor Total de Tributos | Valor Total dos Tributos 
Valor a Receber | Valor a Receber 
Valor Total de Carga | Valor total da carga 

**Fisco** | **Descrição**
----------|--------------
Info.Adicional | Informações adicionais de interesse do Fisco

### Componentes

**Campo** | **Descrição**
----------|---------
Nome | Nome do componente
Valor | Valor do componente 

### Mercadorias

**Campo** | **Descrição**
----------|-------------
Unidade | Código da Unidade de Medida
Tipo de Medida | Tipo da Medida 
Quantidade de Carga | Quantidade 
Valor da Carga para Averbação | Valor da Carga para efeito de averbação 

### Documentos

**Campo** | **Descrição**
----------|--------------
Chave | Chave de acesso da NF-e ou Chave de acesso do CT-e 
NF-e ou Doc. Anterior | NF-e ou Documento Anterior

### Impostos

**Campo** | **Descrição**
----------|---------------
Tipo CST | Tipo do CST
Número CST | Classificação Tributária do Serviço 
Descrição CST | Descrição do CST
Valor BC | Valor da BC do ICMS 
% ICMS | Alíquota do ICMS 
Valor ICMS | Valor do ICMS 
% Redução BC | Percentual de redução da BC 
Valor BC do ICMS ST retido | Valor da BC do ICMS ST retido 
Valor ICMS ST Retido | Valor do ICMS ST retido
% ICMS ST Retido | 
Valor Crédito |
Simples Nacional |
% ICMS FCP |
Valor ICMS FCP |
% ICMS Interestadual |

### Emitente/Remetente/Expedidor/Recebedor/Destinatário

**Campo** | **Descrição**
----------|--------------
Identificador |
Nome |
Marca |
CNPJCPF |
IE |
IEST |
Logradouro |
Número |
Complemento |
Bairro |
Município |
CEP | 
Estado | 
DDD |
Telefone |
Email |

### Seguro

**Campo** | **Descrição**
----------|--------------
Responsável |
Seguradora |
Apólice |
