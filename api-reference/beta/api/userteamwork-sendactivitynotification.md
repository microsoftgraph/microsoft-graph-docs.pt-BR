---
title: 'Conjunto de equipe: sendActivityNotification'
description: Enviar uma notificação de feed de atividades para um usuário.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09e9382663140abbd736a7497ce632bacf83b24b
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377487"
---
# <a name="userteamwork-sendactivitynotification"></a>Conjunto de equipe: sendActivityNotification
Namespace: microsoft.graph

Enviar uma notificação de feed de atividades para um usuário. Para obter mais detalhes sobre o envio de notificações e os requisitos para fazer isso, consulte [enviando notificações de atividade do teams](/graph/teams-send-activityfeednotifications).

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|TeamsActivity.Send|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|TeamsActivity.Send|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/teamwork/sendActivityNotification
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
|topic|[teamworkActivityTopic](../resources/teamworkactivitytopic.md)|Tópico da notificação. Especifica o recurso que está sendo falamos.|
|activityType|Cadeia de caracteres|Tipo de atividade. Isso deve ser declarado no [manifesto do aplicativo Teams](/microsoftteams/platform/overview).|
|chainid|Int64|Opcional. Usado para substituir uma notificação anterior. Use o mesmo `chainId` nas solicitações subsequentes para substituir a notificação anterior.|
|previewText|[itemBody](../resources/itembody.md)|Visualizar o texto da notificação. O Microsoft Teams só mostrará os primeiros 150 caracteres.|
|TemplateParameters|Coleção [keyValuePair](../resources/keyvaluepair.md)|Valores para variáveis de modelo definidas na entrada de feed de atividade correspondente ao `activityType` [manifesto do aplicativo Teams](/microsoftteams/platform/overview).|

Os recursos a seguir têm suporte ao definir o `source` valor da propriedade **topic** como `entityUrl` :

- [teamsAppInstallation](../resources/teamsappinstallation.md)
- [teamsCatalogApp](../resources/teamscatalogapp.md)

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a>Exemplo 1: enviar notificação para um usuário para uma tarefa criada

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "userteamwork_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
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

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a>Exemplo 2: notificar um usuário sobre um evento usando o tópico personalizado

Se você deseja vincular um aspecto que não é representado pelo Microsoft Graph ou deseja personalizar o nome, você pode definir a fonte do `topic` para `text` e passar um valor personalizado para ele. `webUrl` é necessário ao usar `topic` source como `text` .

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification

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
