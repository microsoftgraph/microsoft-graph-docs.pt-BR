---
title: 'timeCard: clockIn'
description: Entre para iniciar um cartão de ponto.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 85c8b917b83bf5285373f0b0684e4295cce4fc7e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989284"
---
# <a name="timecard-clockin"></a>timeCard: clockIn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Clock in to start a [timeCard](../resources/timeCard.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Schedule.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Schedule.ReadWrite.All* |

>\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/clockIn
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório.|
| MS-APP-ACTS-AS | A ID do usuário em nome do qual o aplicativo está agindo. Obrigatório ao usar o escopo de permissão do aplicativo. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|atApprovedLocation| `Edm.boolean ` | Indique se essa ação acontece em um local aprovado.|
|onBehalfOfUserId| Cadeia de caracteres | Parâmetro opcional usado pelo gerente para entrar no relógio em nome de um usuário.|
|notes| [itemBody](../resources/itembody.md)  |Observações para o relógio em. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [timeCard](../resources/timeCard.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação. 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-clockin"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/clockin
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "clock in notes"
    }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-clockin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-clockin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/timecard-clockin-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T22:58:41.327Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedIn",
    "confirmedBy": "none",
    "clockOutEvent": null,
    "notes": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    },
    "clockInEvent": {
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "breaks": [],
    "originalEntry": {
        "clockOutEvent": null,
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "breaks": []
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Clock In",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
