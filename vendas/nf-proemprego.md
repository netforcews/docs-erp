# Emitir uma nota Pró-Emprego

Para emitir uma nota com os padrões descritos pelo Pró-Emprego, siga os seguintes passos:

1. Nos cadastro dos produtos que você deseja inserir na nota, marque a opção ```Pró Emprego```, insira os valores necessários nos campos 
referentes ao ```Pró Emprego``` e salve:

![cadastro-produtos-proemprego](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/cadastro-produtos-proemprego.png)

2. Ainda em cadastros, dirija-se até ```Tabelas```->```ICMSs```, selecione o registro referente a emissão de nota que você deseja fazer e
clique na Aba ```Informações Complementares```:

![cadastro-tabelas](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/cadastro-tabelas.png)
![cadastro-tabelas-icms](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/cadastro-tabelas-icms.png)
![icms-inf](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/icms-inf.png)

3. Preencha os dados para a emissão da nota, caso tenha dúvida sobre o que cada campo se refere deixe o mouse em cima do campo para obter
informações do mesmo. Para informação de uso das variáveis ou das opções olhe no final desse passo-a-passo. Por final, salve:

![inf-comp](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/inf-comp.png)

4. Crie um novo pedido normalmente, então nos itens do pedido insira os produtos que estão configurados para o ```Pró Emprego``` (Passo 1),
na repartição **Impostos** não se esqueça de colocar a classe ```51``` no campo **Class. Tributaria**:

![classtrib](https://raw.githubusercontent.com/netforcews/docs-erp/master/vendas/imgs/classtrib.png)

5. Depois do pedido pronto, você pode fazer a emissão da nota normalmente.

## Opções

- [x] Ativo
> O campo acima está ativo e irá aparecer no xml da nota

- [ ] Ativo
> O campo acima está desativado e não vai aparecer em lugar algum

- [x] Agrupar itens
> Os valores dos itens das notas vão ser somados e adicionados em uma linha só da tag acima. (Essa opção desativa as variáveis **{{pDif}} e {{nItem}}**)

- [ ] Agrupar itens
> Cada item vai ter uma linha com o seus respectivos valores na tag acima.

- [x] Utilizar tag ICMS90
> A tag ICMS90 vai ser adicionada ao xml

- [ ] Utilizar tag ICMS90
> A tag ICMS90 **não** vai ser adicionada ao xml

## Variáveis

As variáveis vão possuir os valores mencionados de cada item, a utilização delas é feita nos valores dos campos **infAdFisco**,
**infCpl - Parcial** e **infCpl - Total**. Em qualquer campo que contiver alguma das 4 variáveis, o lugar que ela está vai ser
substituído pelo valor do item ou a soma dos itens dependendo do preenchimento da opção **Agrupar Itens**.

## Exemplos


### Exemplo de preenchimento do campo **infCpl** e resultado no xml:

- Com **Agrupar Itens** habilitado (variáveis {{pDif}} e {{nItem}} não consideradas nesse caso):

  - **infCpl:** ITENS COM VALOR ICMS DIFERIDO DE {{vICMSDif}} E VALOR ICMS DA OPERACAO DE {{vICMSOp}}

  - **XML**:
```xml
<infCpl>
PED: 00003670. TOTAL APROXIMADO DOS TRIBUTOS: FEDERAIS R$ 2,57 (12,42%) ESTADUAIS R$ 2,38 (11,50%) FONTE IBPT. ITENS COM VALOR ICMS DIFERIDO DE 1,14 E VALOR ICMS DA OPERACAO DE 1,14
</infCpl>
```
> Todos os valores e números são exemplos

- Com **Agrupar Itens** desabilitado:

  - **infCpl:** ITEM N {{nItem}} COM VALOR ICMS DIFERIDO DE {{vICMSDif}}, PERCENTUAL {{pDif}} E VALOR ICMS DA OPERACAO DE {{vICMSOp}}

  - **XML:**
```xml
<infCpl>
PED: 00003673. TOTAL APROXIMADO DOS TRIBUTOS: FEDERAIS R$ 2,57 (12,42%) ESTADUAIS R$ 2,38 (11,50%) FONTE IBPT. ITEM N 1 COM VALOR ICMS DIFERIDO DE 1,14, PERCENTUAL 100 E VALOR ICMS DA OPERACAO DE 1,14. ITEM N 3 COM VALOR ICMS DIFERIDO DE 1,78, PERCENTUAL 100 E VALOR ICMS DA OPERACAO DE 1,78.
</infCpl>
```
> Todos os valores e números são exemplos


### Exemplo de preenchimento do campo **infAdFisco** e resultado no xml:

- **infAdFisco:** ICMS DIFERIDO PRO-EMPREGO, CONFORME DECRETO 104 DE 14/03/07 E RESOLUÇÃO 210/2010-SEF-TTD TTD 105000001716264.

- **XML:**
```xml
<infAdFisco>
ICMS DIFERIDO PRO-EMPREGO, CONFORME DECRETO 104 DE 14/03/07 E RESOLUCAO 210/2010-SEF-TTD TTD 105000001716264.
</infAdFisco>
```
