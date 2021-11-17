---
title: Substituir timeCard
description: Atualize uma entrada de cartão de ponto existente.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b697bf8fd9dfca971c8eef975a0113652a2c9e80
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988948"
---
# <a name="replace-timecard"></a>Substituir timeCard

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Substitua um [cartão](../resources/timecard.md) de ponto existente por valores atualizados.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Schedule.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Schedule.ReadWrite.All*  |

>\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |
| MS-APP-ACTS-AS | A ID do usuário em nome do qual o aplicativo está agindo. Obrigatório ao usar o escopo de permissão do aplicativo. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto timeCard.](../resources/timecard.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard_replace"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_3cd7413f-0337-433b-9a49-da0923185b3f
Content-type: application/json

{
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "None",
    "notes": null,
    "clockInEvent": {
        "dateTime": "2021-05-21T21:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-21T22:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-21T21:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            },
            "end": {
                "dateTime": "2021-05-21T22:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            }
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-replace-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-replace-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-replace-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-replace-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/timecard-replace-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 
<!-- {
  "blockType": "response",
  "name": "timecard_replace"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
