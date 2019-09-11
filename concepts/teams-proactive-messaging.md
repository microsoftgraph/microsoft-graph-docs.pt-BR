---
title: Mensagens pró-ativas usando um bot no Microsoft Teams
description: Enviar uma mensagem proativa para um usuário do Microsoft Teams com um aplicativo personalizado instalando primeiro o bot usando o Microsoft Graph.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a1cdd206d7cc6db97340ec41727ce9ea64c86510
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839196"
---
# <a name="proactive-messaging-using-a-bot-in-microsoft-teams"></a>Mensagens pró-ativas usando um bot no Microsoft Teams

Uma mensagem proativa é uma mensagem enviada a um usuário do Microsoft Teams sem um usuário que inicia a conversa. Aplicativos personalizados no Microsoft Teams podem enviar mensagens pró-ativas para usuários usando um bot. No entanto, para fazer isso, o bot precisa ser instalado como um aplicativo pessoal ou em uma equipe da qual o usuário é membro. Esse requisito pode ser proibitivo em cenários em que você precisará proativamente enviar uma mensagem a um grupo de usuários que podem ou não ter o aplicativo Teams instalado.

Este artigo descreve como você pode combinar o Microsoft Graph com um aplicativo do Microsoft Teams para instalar o aplicativo para seus usuários e, em seguida, usar seu aplicativo Teams para enviar uma mensagem pró-ativa, sem exigir que ele instale o aplicativo manualmente.

Em um nível alto, você precisará:

* [Criar seu aplicativo e bot do Microsoft Teams](#create-your-teams-app-and-bot)
* [Implantar seu aplicativo no catálogo de aplicativos do locatário](#deploy-your-app-to-your-tenant-app-catalog)
* [Instalar o aplicativo para seus usuários](#install-the-app-for-your-users)

## <a name="create-your-teams-app-and-bot"></a>Criar seu aplicativo e bot do Microsoft Teams

Se você ainda não tiver um aplicativo do Microsoft Teams com um bot que possa enviar a mensagem, você precisará criar um. Consulte [Add bots to Teams apps](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-overview) na documentação da plataforma do teams. Para obter informações sobre como criar um bot para mensagens proativas, consulte [Proactive Messaging for bots](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).

Você também pode usar o [modelo de aplicativo Company Communicator](https://github.com/OfficeDev/microsoft-teams-company-communicator-app) como um bom ponto de partida para seu aplicativo. Este modelo de aplicativo é um aplicativo Microsoft Teams pronto para produção capaz de criar, agendar e distribuir mensagens em toda a empresa.

Ao criar seu aplicativo, certifique-se de anotar o `id` que você usa em seu manifesto de aplicativo; Você precisará dele para instalar o aplicativo em uma etapa posterior.

Se você estiver fazendo isso para uma organização de grande porte, as mensagens de boas-vindas do seu bot podem ser limitadas. Se possível, execute as instalações em lotes e implemente a funcionalidade de back-out no bot. Para obter detalhes, consulte [tratamento da limitação da taxa](/microsoftteams/platform/concepts/bots/rate-limit).

## <a name="deploy-your-app-to-your-tenant-app-catalog"></a>Implantar seu aplicativo no catálogo de aplicativos do locatário

O Microsoft Graph só pode instalar aplicativos que foram adicionados ao catálogo de aplicativos de locatários ou estão disponíveis no repositório de aplicativos públicos do Microsoft Teams. Se você estiver trabalhando com um novo aplicativo, será necessário verificar se ele é o [Catálogo de aplicativos do locatário](https://docs.microsoft.com/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog).

## <a name="install-the-app-for-your-users"></a>Instalar o aplicativo para seus usuários

Para instalar o aplicativo Teams para seus usuários, primeiro você precisará garantir que o seu aplicativo do Microsoft Graph tenha as permissões corretas – você precisará de User. ReadWrite. All ou Directory. ReadWrite. All para instalar o aplicativo Teams. Você também precisará de chat. Read. All para uma etapa posterior. As duas permissões exigirão o consentimento do administrador e você precisará usar permissões de aplicativo, em vez de usuário delegadas, porque você instalará aplicativos para usuários que não são de sua conta.

### <a name="check-to-see-if-the-app-is-already-installed"></a>Verifique se o aplicativo já está instalado

Primeiro, convém verificar se o aplicativo de equipes já está instalado para os usuários dos quais você deseja instalá-lo, conforme mostrado no exemplo.

```http
GET /users/{user-id}/teamwork/installedApps?$expand=teamsAppDefinition&$filter=teamsAppDefinition/teamsAppId eq '{teamsAppid}'
```

Em `{teamsAppId}` que é `id` o manifesto do aplicativo Teams que você fez anotar anteriormente. Observe que isso pode ser diferente das chamadas `appid` para o Microsoft Graph e do seu `botId`. Você pode achar útil instalar manualmente o aplicativo para um usuário e testar a chamada em relação a esse usuário para garantir que você tem o valor correto `id` .

A chamada retornará uma matriz vazia se o aplicativo não estiver instalado ou uma matriz com um único [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) se já estiver instalada.

### <a name="install-the-app"></a>Instalar o aplicativo

Se o aplicativo ainda não estiver instalado para esse usuário, você poderá instalá-lo, conforme mostrado no exemplo a seguir.

```http
POST /users/{user-id}/teamwork/installedApps
{
   "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppid}"
}
```

Para obter mais informações, consulte [install App for User](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta).

Se o usuário tiver o Microsoft Teams em execução, ele poderá ou não ver a instalação do aplicativo imediatamente – talvez seja necessário reiniciar o aplicativo para ver a instalação.

## <a name="get-the-chat-thread-id"></a>Obter a ID do thread de chat

Quando o aplicativo é instalado para o usuário, o bot receberá um `conversationUpdate` evento que conterá as informações necessárias para enviar a mensagem proativa. Para mais informações, consulte [eventos de bot](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-notifications).

Se você perder o `chatThreadId`, poderá encontrá-lo novamente chamando:

```http
GET /users/{user-id}/chats?$filter=installedApps/any(a:a/teamsApp/id eq '{teamsAppid}'
```

A propriedade **ID** do resultado é a ID chatThread.

## <a name="sending-the-message"></a>Envio da mensagem

Agora que seu bot tem as informações necessárias, você pode [Enviar uma mensagem proativa](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).

## <a name="c-sample"></a>Exemplo de C#

Consulte https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg (Observe a ramificação).
O código interessante está `InstallAppToAllUsers()` no [GraphService.cs](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs).
