---
title: 'chat: sendActivityNotification'
description: Envie uma notificação de feed de atividades no escopo de um chat.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7147ad0019b9c066f19f30b9829e80e1a75570ca
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872856"
---
# <a name="chat-sendactivitynotification"></a>chat: sendActivityNotification
Namespace: microsoft.graph

Envie uma notificação de feed de atividades no escopo de um chat. Para obter mais detalhes sobre como enviar notificações e os requisitos para fazer isso, confira [o envio de notificações de atividades do Teams.](/graph/teams-send-activityfeednotifications)

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
POST /chats/{chatId}/sendActivityNotification
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
|activityType|Cadeia de caracteres|Tipo de atividade. Isso deve ser declarado no manifesto do [aplicativo Teams.](/microsoftteams/platform/overview)|
|chainId|Int64|Opcional. Usado para substituir uma notificação anterior. Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.|
|previewText|[itemBody](../resources/itembody.md)|Texto de visualização para a notificação. O Microsoft Teams mostrará apenas os primeiros 150 caracteres.|
|templateParameters|Coleção [keyValuePair](../resources/keyvaluepair.md)|Valores para variáveis de modelo definidos na entrada do feed de atividades correspondente no `activityType` manifesto do aplicativo do [Teams.](/microsoftteams/platform/overview)|
|destinatário|[teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md)|Destinatário da notificação. Somente os usuários do Azure AD têm suporte. Consulte também [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md). |

Os seguintes recursos são suportados ao definir `source` o valor da propriedade **de** tópico `entityURL` como:

- [chat](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

> **Observação:** A URL da entidade deve ser igual ou um recurso filho do chat na URL. Além disso, o [aplicativo Teams](/microsoftteams/platform/overview) deve ser instalado no chat.

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>Exemplo 1: Notificar um usuário sobre uma tarefa criada em um chat

Este exemplo mostra como você pode enviar uma notificação de feed de atividades para uma nova tarefa criada em um chat. Para obter mais detalhes, confira [o envio de notificações de atividades do Teams.](/graph/teams-send-activityfeednotifications)

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

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

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a>Exemplo 2: Notificar um usuário sobre uma aprovação necessária em uma mensagem de chat

Semelhante ao exemplo anterior, este exemplo usa `entityUrl` para `topic` o . No entanto, nesse caso, ele é links para uma mensagem no chat. A mensagem pode conter um cartão com o botão de aprovação.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "Deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "approvalTaskId",
            "value": "2020AAGGTAPP"
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

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a>Exemplo 3: Notificar um usuário sobre um evento em relação a um chat

Conforme mostrado nos exemplos anteriores, você pode vincular a diferentes aspectos do chat. No entanto, se você deseja vincular a um aspecto que não faz parte do chat ou não é representado pelo Microsoft Graph, você pode definir a origem do para e passar um valor personalizado `topic` `text` para ele. Além disso, `webUrl` é necessário ao definir a fonte como `topic` `text` .

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
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
