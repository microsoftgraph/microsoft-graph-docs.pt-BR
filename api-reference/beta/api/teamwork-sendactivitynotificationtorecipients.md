---
title: 'trabalho em equipe: sendActivityNotificationToRecipients'
description: Enviar notificações do feed de atividades para vários usuários em massa.
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 715d5daf735b7eb79b48468db53339d860ea4feb
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445164"
---
# <a name="teamwork-sendactivitynotificationtorecipients"></a>trabalho em equipe: sendActivityNotificationToRecipients

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enviar notificações do feed de atividades para vários usuários, em massa. 

Para obter mais detalhes sobre como enviar notificações e os requisitos para fazer isso, consulte [enviar notificações de atividades do Teams](/graph/teams-send-activityfeednotifications).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegada (conta corporativa ou de estudante)     | TeamsActivity.Send                          |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | TeamsActivity.Send                          |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /teamwork/sendActivityNotificationToRecipients
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

| Parâmetro          | Tipo                                                         | Descrição                                                  |
| :----------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| topic              | [teamworkActivityTopic](../resources/teamworkactivitytopic.md) | Tópico da notificação. Especifica o recurso que está sendo falado. |
| activityType       | Cadeia de caracteres                                                       | Tipo de atividade. Isso deve ser declarado no manifesto [do aplicativo Teams](/microsoftteams/platform/overview). |
| chainId            | Int64                                                        | Opcional. Usado para substituir uma notificação anterior. Use o mesmo em `chainId` solicitações subsequentes para substituir a notificação anterior. |
| previewText        | [itemBody](../resources/itembody.md)                         | Visualizar texto para a notificação. O Microsoft Teams mostrará apenas os primeiros 150 caracteres. |
| Templateparameters | Coleção [keyValuePair](../resources/keyvaluepair.md)      | Valores para variáveis de modelo definidos na entrada do feed de atividades correspondentes ao `activityType` manifesto [do aplicativo Teams](/microsoftteams/platform/overview). |
| teamsAppId         | String                                                       | Opcional. ID do aplicativo Teams do aplicativo Teams associado à notificação. Usado para desambiguar aplicativos instalados quando vários aplicativos com a mesma Azure AD ID do aplicativo são instalados para o mesmo usuário destinatário. |
| destinatários         | [Coleção teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md) | Destinatários da notificação. Somente os destinatários do [tipo aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) têm suporte. Há um limite superior de 100 destinatários em uma única solicitação. |

O recurso a seguir tem suporte ao definir o `source` valor da propriedade **de** tópico como `entityUrl`:

- [teamsCatalogApp](../resources/teamscatalogapp.md)

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

## <a name="examples"></a>Exemplos

### <a name="example-1-notify-multiple-users-about-pending-finance-approval-requests"></a>Exemplo 1: notificar vários usuários sobre solicitações de aprovação de finanças pendentes

O exemplo a seguir mostra como enviar uma notificação do feed de atividades para vários usuários em massa. Este exemplo notifica vários stakeholders sobre solicitações de aprovação de finanças pendentes.

#### <a name="request"></a>Solicitação



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients_1"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ],
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamwork-sendactivitynotificationtorecipients-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamwork-sendactivitynotificationtorecipients-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamwork-sendactivitynotificationtorecipients-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/teamwork-sendactivitynotificationtorecipients-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/teamwork-sendactivitynotificationtorecipients-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false
}
-->

``` http
HTTP/1.1 202 Accepted
```

### <a name="example-2-notify-multiple-users-about-an-event-using-a-custom-topic"></a>Exemplo 2: Notificar vários usuários sobre um evento usando um tópico personalizado

Se você quiser vincular um aspecto que não é representado pelo Microsoft Graph ou quiser personalizar o nome, `topic` `text` poderá definir a origem e passar um valor personalizado para ele. `webUrl` é necessário ao usar a origem `topic` como `text`.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients_2"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
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
    ],
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamwork-sendactivitynotificationtorecipients-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamwork-sendactivitynotificationtorecipients-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamwork-sendactivitynotificationtorecipients-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/teamwork-sendactivitynotificationtorecipients-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/teamwork-sendactivitynotificationtorecipients-2-powershell-snippets.md)]
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
HTTP/1.1 202 Accepted
```
