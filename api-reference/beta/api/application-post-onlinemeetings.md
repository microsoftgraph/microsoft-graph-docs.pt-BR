---
title: Criar reunião online
description: Cria uma reunião online em nome de um usuário específico no corpo da solicitação.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: bd4d68a5e93e9b1b0afe91129d83e40135e79cbf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258426"
---
# <a name="create-online-meeting"></a>Criar reunião online

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cria uma reunião online em nome de um usuário específico no corpo da solicitação.

> **Observação**: a reunião não é exibida no calendário do usuário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Não suportado                               |
| Delegado (conta pessoal da Microsoft) | Não suportado                               |
| Aplicativo                            | OnlineMeetings.ReadWrite.All                |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto [onlineMeeting](../resources/onlinemeeting.md).

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/onlineMeetings
Content-Type: application/json
Content-Length: 1553

{
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  "subject": "subject-value"
}
```

No corpo da solicitação, forneça uma representação JSON do objeto [onlineMeeting](../resources/onlinemeeting.md).

##### <a name="response"></a>Resposta

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1574

{
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "participantPasscode": "2425999",
    "leaderPasscode": null,
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": "2018-03-19T09:46:02Z",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2018-03-19T09:46:02Z",
  "endDateTime": "2018-03-19T09:46:02Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "013448345",
  "isCancelled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-03-19T09:46:02Z",
  "subject": "Quarterly sales numbers"
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
