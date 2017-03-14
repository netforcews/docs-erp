# Erro Bad Request
## Problema
Você está tentando acessar o seu sistema **NetForce** e o navegador lhe mostra uma mensagem com o título **Bad Request**.

## Causa
Esse problema é causado devido ao excesso de cookies em seu navegador, esses cookies ficam sobrecarregados e não conseguem ser processados
pelo servidor retornando a devida mensagem de erro **Bad Request**.

## Solução
Para resolver esse problema o processo é bem simples, você apenas precisa apagar seus cookies, para fazer isso siga os seguintes passos:

### Google Chrome

1- Primeiramente, acesse o seu sistema, a página do **Bad Request** vai aparecer, então clique com o botão direito em qualquer lugar da
tela e navegue até a opção **Inspecionar**, ou simplesmente aperte ```Ctrl+Shift+I```:

![botao-direito](https://raw.githubusercontent.com/netforcews/docs-erp/master/erros/imgs/botao-direito.jpg)

2- No menu que aparece, clique na opção **Application**:

![application](https://raw.githubusercontent.com/netforcews/docs-erp/master/erros/imgs/application.png)

3- Procure pela opção **Cookies** (geralmente você precisa descer um pouco a barra de rolagem), assim que achar clique na setinha do botão
de **Cookies**:

![barra-de-rolagem](https://raw.githubusercontent.com/netforcews/docs-erp/master/erros/imgs/barra-de-rolagem.png)

![cookies-setinha](https://raw.githubusercontent.com/netforcews/docs-erp/master/erros/imgs/cookies-setinha.png)

4- Assim que clicar na setinha você irá ver ```http://dws.netforce.com.br```, clique nessa opção e vários registros de cookies aparecerão
na janela ao lado do menu lateral da esquerda. Clique em cima de qualquer um dos registros e apague todos da maneira que você quiser:

![cookie-dws-cookies](https://raw.githubusercontent.com/netforcews/docs-erp/master/erros/imgs/cookie-dws-cookies.png)

5- Feito isso você pode fechar o menu do **Inspecionar** e apertar ```F5``` para recarregar a página, você vai ver que irá aparecer na tela
a interface de login da **NetForce**, apenas faça seu login que o sistema agora já está normal novamente:

![login](https://raw.githubusercontent.com/netforcews/docs-erp/master/erros/imgs/login.png)
