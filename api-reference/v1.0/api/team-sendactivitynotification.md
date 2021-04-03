---
title: 'team: sendActivityNotification'
description: Envie uma notificação de feed de atividade no escopo de uma equipe.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: add05d086580d5ed76b4195de98d28187e3ad30d
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507554"
---
# <a name="team-sendactivitynotification"></a>team: sendActivityNotification
Namespace: microsoft.graph

Envie uma notificação de feed de atividade no escopo de uma equipe. Para obter mais detalhes sobre como enviar notificações e os requisitos para fazer isso, consulte [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|TeamsActivity.Send|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|TeamsActivity.Send|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|topic|[teamworkActivityTopic](../resources/teamworkactivitytopic.md)|Tópico da notificação. Especifica o recurso que está sendo falado.|
|activityType|Cadeia de caracteres|Tipo de atividade. Isso deve ser declarado no manifesto do [aplicativo teams.](/microsoftteams/platform/overview)|
|chainId|Int64|Opcional. Usado para substituir uma notificação anterior. Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.|
|previewText|[itemBody](../resources/itembody.md)|Visualizar texto para a notificação. O Microsoft Teams mostrará apenas os primeiros 150 caracteres.|
|templateParameters|Coleção [keyValuePair](../resources/keyvaluepair.md)|Valores para variáveis de modelo definidas na entrada de feed de atividade correspondente `activityType` ao manifesto do aplicativo do [Teams.](/microsoftteams/platform/overview)|
|destinatário|[teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md)|Destinatário da notificação. Somente usuários do Azure AD são suportados. Consulte também [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md). |

Os seguintes recursos são suportados ao definir o `source` valor da propriedade **topic** como `entityUrl` :

- [team](../resources/team.md)
- [channel](../resources/channel.md)
- [chatMesage](../resources/chatmessage.md)
- [teamsTab](../resources/teamstab.md)

> **Observação:** A URL da entidade deve ser o mesmo ou o recurso filho da equipe na URL. Além disso, o [aplicativo do Teams](/microsoftteams/platform/overview) deve ser instalado na equipe.

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a>Exemplo 1: Notificar um usuário sobre solicitações pendentes de aprovação de finanças

Este exemplo mostra como você pode enviar uma notificação de feed de atividade para uma equipe. Este exemplo notifica o proprietário da equipe sobre solicitações pendentes de aprovação de finanças.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a>Exemplo 2: Notificar um usuário sobre uma guia de canal

Semelhante ao exemplo anterior, este exemplo usa `entityUrl` para `topic` o . No entanto, este exemplo se vincula a [uma guia](../resources/teamstab.md) em um [canal](../resources/channel.md). A guia hospeda uma página mostrando ao usuário o status de sua reserva de hotel. Selecionar a notificação levará o usuário para a guia, onde ele pode verificar sua reserva.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    },
    "activityType": "reservationUpdated",
    "previewText": {
        "content": "You have moved up the queue"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "reservationId",
            "value": "TREEE433"
        },
        {
            "name": "currentSlot",
            "value": "23"
        }
    ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a>Exemplo 3: Notificar um usuário sobre um evento usando tópico personalizado

Como visto nos exemplos anteriores, você pode vincular a diferentes aspectos da equipe. No entanto, se você deseja vincular a um aspecto que não faz parte da equipe ou não é representado pelo Microsoft Graph, ou deseja personalizar o nome, você pode definir a origem do para e passar um valor personalizado para `topic` `text` ele. `webUrl` é necessário ao definir `topic` a fonte como `text` .

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "deploymentApprovalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
