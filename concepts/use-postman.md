---
title: Use o Postman com a API do Microsoft Graph
description: Use a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: b5dbeb6c779bcd02cd1ae329b3b63df6c44a1da8
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430127"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>Use o Postman com a API do Microsoft Graph

Você pode usar a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.

![Imagem do Postman](images/postman-screenshot.png)

Este artigo explica como começar a usar o Postman e o Microsoft Graph. Você também pode explorar as APIs do Microsoft Graph diretamente em seu navegador da Web usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Para obter detalhes sobre como fazer isso, siga as etapas deste artigo ou assista ao vídeo [Introdução ao espaço de trabalho do Postman no Microsoft Graph](https://youtu.be/3RTHY3jScmA).

## <a name="step-1---forking-the-microsoft-graph-postman-collection"></a>Etapa 1 - Bifurcação da coleção do Microsoft Graph Postman

Para usar a coleção do Postman, bifurque-a no próprio espaço de trabalho do Postman. Faça isso no navegador da Web.

1. Vá para [Postman](https://www.postman.com/) e conecte-se.
1. Vá para a coleção do [Postman](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork) rotulada Microsoft Graph.
1. Preencha um rótulo com sua própria bifurcação de repositório. Pode ser qualquer texto.
1. No espaço de trabalho, certifique-se de que **Meu espaço de trabalho** esteja selecionado na lista suspensa.
1. Clique em **Coleção de bifurcação de repositório**.

Você será redirecionado para uma bifurcação da coleção principal do Microsoft Graph Postman no próprio espaço de trabalho.

## <a name="step-2---optional---postman-web-browser-only-download-the-postman-agent"></a>Etapa 2 - (Opcional - Apenas navegador da Web Postman) Baixar o agente Postman

Para usar esta coleção específica do Postman em seu navegador, baixe o [Agente de área de trabalho Postman](https://www.postman.com/downloads). Não é possível usar o Postman para a Web sem isso devido às restrições de CORS do navegador.

Você não precisa do agente se estiver usando o aplicativo Postman para Windows. Se você abrir o Postman para Windows, verá essa coleção bifurcada em seu espaço de trabalho.

## <a name="step-3---create-an-azure-ad-application"></a>Etapa 3 - Criar um aplicativo do Azure AD

Para usar essa coleção no próprio locatário de desenvolvedor, crie um aplicativo do Azure AD e conceda a ele as permissões apropriadas para as solicitações que deseja chamar. Se você não tiver um locatário de desenvolvedor, poderá se inscrever para obter um por meio do [Programa para Desenvolvedores do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).

1. Vá até o [portal.azure.com](https://portal.azure.com/) e entre com sua conta de administrador de locatários de desenvolvedor.
1. Em **Serviços do Azure**, clique em **Azure Active Directory**.
1. No menu à esquerda, clique em **Registros de aplicativo**.
1. No menu horizontal, clique em **Novo registro**.
1. Defina o **Nome do aplicativo** como `Postman`.
1. Defina a **URI de redirecionamento** como`https://oauth.pstmn.io/v1/browser-callback`.
1. Clique em **Registrar**.
1. No menu à esquerda, clique em **Permissões de API**.
1. No menu horizontal, clique em **Adicionar uma permissão**, selecione **Microsoft Graph**, em seguida, selecione **Permissões delegadas**.
1. Digite `Mail.`, expanda as opções de **Email** e marque **Mail.Read**.
1. Clique em **Permissões de aplicativo**, digite `User.`e verifique as **Permissões de aplicativo**.
1. Expanda as opções de **Usuário** e marque **User.Read.All**.
1. Clique em **Adicionar permissões**.
1. No menu horizontal, clique em **Conceder consentimento de administração** e clique em **Sim**.
1. No menu à esquerda, clique em **Visão geral**. A partir daqui, você poderá obter a **ID de aplicativo (cliente)** e a **ID de diretório (locatário)**. Você precisará delas na etapa 4.
1. No menu à esquerda, clique em **Certificados e segredos**.
1. Selecione **Novo segredo do cliente**, insira uma descrição e selecione **Adicionar**. Passe o mouse sobre o novo **Valor** do segredo do cliente e copie-o. Você precisará dele na etapa 4.

O aplicativo do Azure AD agora tem permissões para fazer solicitações em nome de um usuário para chamar Mail.Read e como aplicativo do User.Read.All.

## <a name="step-4---configuring-authentication-in-postman"></a>Etapa 4 - Configurando autenticação no Postman

Nesta etapa, você irá configurar as variáveis do ambiente usadas para recuperar um token de acesso.

1. Vá para o [ambiente de Bifurcação](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/environment/455214-efbc69b2-69bd-402e-9e72-850b3a49bb21/fork).
1. Adicionar um rótulo para a bifurcação. Pode ser qualquer texto.
1. No espaço de trabalho, certifique-se de que **Meu espaço de trabalho** esteja selecionado na lista suspensa.
1. Clique em **ambiente de Bifurcação**.
1. Em `ClientID`, defina o **Valor atual** como o valor da ID de aplicativo (cliente) da etapa 3.15.
1. Em `ClientSecret`, defina o **Valor atual** para o valor do segredo do cliente da etapa 3.17.
1. Em`TenantID`, defina o **Valor atual** como o valor da ID de diretório (locatário) da etapa 3.15.
1. No canto superior direito, clique em **Salvar**.
1. Feche a guia **Gerenciar ambientes**.
1. No canto superior direito, próximo ao ícone de olho, verifique se o **Ambiente M365** está selecionado no menu suspenso e não em **Nenhum ambiente**.

## <a name="step-5---get-a-delegated-access-token"></a>Etapa 5 - Obter um token de acesso delegado

Como esta é a primeira vez que você está executando uma solicitação como um fluxo de autenticação delegado, é necessário obter um token de acesso.

1. Passe o mouse sobre a pasta **Delegado**, clique nas reticências e selecione **Editar**
1. Clique na guia **Autorização**.
1. Role para baixo à direita e clique em **Obter novo token de acesso**.
1. Entre com sua conta de administrador de locatários de desenvolvedor.
1. Clique em **Prosseguir** e, em seguida, clique no botão **Usar token**.
1. Na parte inferior direita da caixa de diálogo, clique em **Atualizar**.

Agora você tem um token de acesso válido para usar para solicitações delegadas.

## <a name="step-6---run-your-first-delegated-request"></a>Etapa 6 - Executar a primeira solicitação delegada

Dentro da pasta **Delegado** estão as solicitações de várias cargas de trabalho do Microsoft Graph que você pode chamar.

1. Expanda a pasta **Delegado**, em seguida, expanda a pasta **Email**.
1. Clique duas vezes em **Obter minhas mensagens** para abrir a solicitação.
1. No canto superior direito, clique em **Enviar**.

Agora você fez uma chamada do Microsoft Graph usando autenticação delegada com êxito.

## <a name="step-7---get-an-application-access-token"></a>Etapa 7 - Obter um token de acesso de aplicativo

Como esta é a primeira vez que você está executando uma solicitação como um fluxo de autenticação de aplicativo, é necessário obter um token de acesso.

1. Passe o mouse sobre a pasta **Aplicativo**, clique nas reticências e selecione **Editar**.
1. Selecione a guia **Autorização**
1. Role para baixo no lado direito e clique em **Obter novo token de acesso**.
1. Clique em **Prosseguir** e, em seguida, clique no botão **Usar token**.
1. Na parte inferior direita da caixa de diálogo, clique em **Atualizar**.

Agora você tem um token de acesso válido para usar para solicitações de aplicativo.

## <a name="step-8---run-your-first-application-request"></a>Etapa 8 - Executar a primeira solicitação de aplicativo

Dentro da pasta **Aplicativo** estão solicitações de várias cargas de trabalho do Microsoft Graph que você pode chamar.

1. Expanda a pasta **Aplicativo** e, em seguida, expanda a pasta **Usuário**.
1. Clique duas vezes em **Obter usuários** para abrir a solicitação.
1. No canto superior direito, clique em **Enviar**.

Agora você fez uma chamada do Microsoft Graph usando a autenticação de aplicativo com êxito.

Você pode seguir essas etapas para fazer outras solicitações para Microsoft Graph. Lembre-se de que você precisa adicionar permissões ao seu aplicativo do Azure AD para que outras solicitações funcionem; Caso contrário, você obterá erros de permissão negada em suas respostas.

### <a name="contribute-to-the-collection"></a>Contribuir com a coleção

Se você quiser contribuir com seus próprios pedidos, precisará de uma licença do Postman. Você pode fazer alterações na coleção bifurcada e, em seguida, passar o mouse sobre o nó superior da coleção e selecionar **Criar solicitação de pull**.

## <a name="see-also"></a>Confira também

Para obter detalhes sobre como fazer isso, assista ao vídeo [Introdução à coleção do Microsoft Graph Postman](https://youtu.be/3RTHY3jScmA).
