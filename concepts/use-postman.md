---
title: Use o Postman com a API do Microsoft Graph
description: Use a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 34be5bab88acbd7545caa958db0809a010660fb4
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059683"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>Use o Postman com a API do Microsoft Graph
Você pode usar a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.

![Imagem do Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

Este artigo explica como começar a usar o Postman e o Microsoft Graph. Você também pode explorar as APIs do Microsoft Graph diretamente em seu navegador da Web usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Para obter detalhes sobre como fazer isso, siga as etapas deste artigo ou assista ao vídeo [Introdução ao espaço de trabalho do Postman no Microsoft Graph](https://youtu.be/3RTHY3jScmA).


## <a name="step-1---forking-the-microsoft-graph-postman-collection"></a>Etapa 1 - Bifurcação da coleção do Microsoft Graph Postman
Para usar a coleção do Postman, bifurque-a no próprio espaço de trabalho do Postman. Faça isso no navegador da Web.

1. Vá para [Postman](https://www.postman.com/) e conecte-se.
2. Vá para a coleção do [Postman](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork) rotulada Microsoft Graph.
3. Preencha um rótulo com sua própria bifurcação de repositório. Pode ser qualquer texto.
4. No espaço de trabalho, certifique-se de que **Meu espaço de trabalho** esteja selecionado na lista suspensa. 
5. Clique em **Coleção de bifurcação de repositório**.

Você será redirecionado para uma bifurcação da coleção principal do Microsoft Graph Postman no próprio espaço de trabalho.

## <a name="step-2---optional---postman-web-browser-only-download-the-postman-agent"></a>Etapa 2 - (Opcional - Apenas navegador da Web Postman) Baixar o agente Postman
Para usar esta coleção específica do Postman em seu navegador, baixe o [Agente de área de trabalho Postman](https://www.postman.com/downloads). Não é possível usar o Postman para a Web sem isso devido às restrições de CORS do navegador. 

Você não precisa do agente se estiver usando o aplicativo Postman para Windows. Se você abrir o Postman para Windows, verá essa coleção bifurcada em seu espaço de trabalho.

## <a name="step-3---create-an-azure-ad-application"></a>Etapa 3 - Criar um aplicativo do Azure AD
Para usar essa coleção no próprio locatário de desenvolvedor, crie um aplicativo do Azure AD e conceda a ele as permissões apropriadas para as solicitações que deseja chamar. Se você não tiver um locatário de desenvolvedor, poderá se inscrever para obter um por meio do [Programa para Desenvolvedores do Microsoft 365](https://developer.microsoft.com/pt-BR/microsoft-365/dev-program).

1. Vá até o [portal.azure.com](https://portal.azure.com/) e entre com sua conta de administrador de locatários de desenvolvedor.
2. Em **Serviços do Azure**, clique em **Azure Active Directory**.
3. No menu à esquerda, clique em **Registros de aplicativo**.
4. No menu horizontal, clique em **Novo registro**.
5. Defina o **Nome do aplicativo** como `Postman`.
6. Defina a **URI de redirecionamento** como`https://oauth.pstmn.io/v1/browser-callback`.
7. Clique em **Registrar**.
8. No menu à esquerda, clique em **Permissões de API**.
9. No menu horizontal, clique em **Adicionar uma permissão**, selecione **Microsoft Graph**, em seguida, selecione **Permissões delegadas**.
10. Digite `Mail.`, expanda as opções de **Email** e marque **Mail.Read**.
11. Clique em **Permissões de aplicativo**, digite `User.`e verifique as **Permissões de aplicativo**.
12. Expanda as opções de **Usuário** e marque **User.Read.All**.
13. Clique em **Adicionar permissões**.
14. No menu horizontal, clique em **Conceder consentimento de administração** e clique em **Sim**.
15. No menu à esquerda, clique em **Visão geral**. A partir daqui, você poderá obter a **ID de aplicativo (cliente)** e a **ID de diretório (locatário)**. Você precisará delas na etapa 4.
16. No menu à esquerda, clique em **Certificados e segredos**. 
17. Selecione **Novo segredo do cliente**, insira uma descrição e selecione **Adicionar**. Passe o mouse sobre o novo **Valor** do segredo do cliente e copie-o. Você precisará dele na etapa 4.

O aplicativo do Azure AD agora tem permissões para fazer solicitações em nome de um usuário para chamar Mail.Read e como aplicativo do User.Read.All.

## <a name="step-4---configuring-authentication"></a>Etapa 4 - Configurando a autenticação
Configure algumas variáveis ​​de ambiente usadas para recuperar um token de acesso.

1. Clique no ícone de olho no canto superior direito próximo ao menu suspenso **Nenhum ambiente**.
2. Clique em **Adicionar** no canto superior direito desse pop-up.
3. Altere **Novo ambiente** para **Ambiente M365**.
4. Crie uma nova variável chamada `ClientID` e defina o **Valor atual** como o valor da ID de aplicativo (cliente) da etapa 3.15.
5. Crie uma nova variável chamada `ClientSecret` e defina o **Valor atual** como o valor do segredo do cliente da etapa 3.17.
6. Crie uma nova variável chamada `TenantID` e defina o **Valor atual** como o valor da ID de diretório (locatário) da etapa 3.15.
7. Selecione **Salvar**/**Atualizar**. 
8. Feche a caixa de diálogo **Gerenciar ambientes**. 
9. Verifique se o **Ambiente M365** está selecionado no menu suspenso e não em **Nenhum ambiente**.

## <a name="step-5---get-a-delegated-access-token"></a>Etapa 5 - Obter um token de acesso delegado
Como esta é a primeira vez que você está executando uma solicitação como um fluxo de autenticação delegado, é necessário obter um token de acesso.

1. Passe o mouse sobre a pasta **Em nome de um usuário**, clique nas reticências e selecione **Editar**
2. Clique na guia **Autorização**.
3. Role para baixo à direita e clique em **Obter novo token de acesso**.
4. Entre com sua conta de administrador de locatários de desenvolvedor.
5. Clique em **Prosseguir** e, em seguida, clique no botão **Usar token**.
6. Na parte inferior direita da caixa de diálogo, clique em **Atualizar**.

Agora você tem um token de acesso válido para usar para solicitações delegadas.

## <a name="step-6---run-your-first-delegated-request"></a>Etapa 6 - Executar a primeira solicitação delegada
Dentro da pasta **Em nome de um usuário** estão solicitações de várias cargas de trabalho do Microsoft Graph que você pode chamar.

1. Expanda a pasta **Em nome de um usuário**, em seguida, expanda a pasta **Email**.
2. Clique duas vezes em **Obter minhas mensagens** para abrir a solicitação.
3. No canto superior direito, clique em **Enviar**.

Agora você fez uma chamada do Microsoft Graph usando autenticação delegada com êxito.

## <a name="step-7---get-an-application-access-token"></a>Etapa 7 - Obter um token de acesso de aplicativo
Como esta é a primeira vez que você está executando uma solicitação como um fluxo de autenticação de aplicativo, é necessário obter um token de acesso.

1. Passe o mouse sobre a pasta **Aplicativo**, clique nas reticências e selecione **Editar**.
2. Selecione a guia **Autorização**
3. Role para baixo no lado direito e clique em **Obter novo token de acesso**.
5. Clique em **Prosseguir** e, em seguida, clique no botão **Usar token**.
6. Na parte inferior direita da caixa de diálogo, clique em **Atualizar**.

Agora você tem um token de acesso válido para usar para solicitações de aplicativo.

## <a name="step-8---run-your-first-application-request"></a>Etapa 8 - Executar a primeira solicitação de aplicativo
Dentro da pasta **Aplicativo** estão solicitações de várias cargas de trabalho do Microsoft Graph que você pode chamar.

1. Expanda a pasta **Aplicativo** e, em seguida, expanda a pasta **Usuário**.
2. Clique duas vezes em **Obter usuários** para abrir a solicitação.
3. No canto superior direito, clique em **Enviar**.

Agora você fez uma chamada do Microsoft Graph usando a autenticação de aplicativo com êxito.

Você pode seguir essas etapas para fazer outras solicitações ao Microsoft Graph. Lembre-se de que você precisa adicionar permissões ao seu aplicativo do Azure AD para que outras solicitações funcionem; Caso contrário, você obterá erros de permissão negada em suas respostas.

### <a name="contribute-to-the-collection"></a>Contribuir com a coleção
Se você quiser contribuir com seus próprios pedidos, precisará de uma licença do Postman. Você pode fazer alterações na coleção bifurcada e, em seguida, passar o mouse sobre o nó superior da coleção e selecionar **Criar solicitação de pull**.

## <a name="see-also"></a>Confira também

Para obter detalhes sobre como fazer isso, assista ao vídeo [Introdução ao espaço de trabalho do Microsoft Graph Postman](https://youtu.be/3RTHY3jScmA).


