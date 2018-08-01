# 778: Informado NCM inexistente

## Causa
Quando for emitida uma NF-e e o NCM (Nomenclatura Comum do Mercosul) não existir na tabela de NCM publicada pelo 
Ministério do Desenvolvimento, Indústria e Comércio Exterior - MDIC, será retornado a rejeição "778 - Informado NCM inexistente".

### Exceções
1. A regra de validação 778 não se aplica, em produção, para NF-e com Data de Emissão anterior a 01/01/2016;
2. Para a NF-e, considerar nesta validação os códigos de NCM especiais definidos pela RFB para permitir o uso no 
Registro de Exportação (Anexo X.02).

## Solução
Para resolver esse problema você precisa verificar o NCM dos itens da nota, caso precise consulte sua contabilidade.
