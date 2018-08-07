# 241: Um número da faixa já foi utilizado

## Causa
Quando for realizada a inutilização de uma numeração já utilizada, será retornado a rejeição 241.
Não se pode inutilizar numerações de NF-e quando já foram Autorizadas, Canceladas, Denegadas ou quando há um Evento EPEC vinculado a numeração, mesmo que a NF-e ainda não tenha sido autorizada.   
Exemplo: Foi emitida uma NF-e, que foi denegada por irregularidade do destinatário. Em seguida, o emissor da NF-e realizou a inutilização da numeração. Nessa situação, a Inutilização será rejeitada pelo motivo 241.

## Solução
Não há nada que possa ser feito para reverter a rejeição da inutilização.
