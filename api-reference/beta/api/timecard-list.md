---
title: Listar timeCard
description: Recupere uma lista de entradas timeCard na agenda.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f6d99e8c4ac38b5238365f8cd49896a924f43e8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989151"
---
# <a name="list-timecard"></a>Listar timeCard

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar uma lista de [entradas timeCard](../resources/timecard.md) em um [cronograma](../resources/schedule.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Schedule.Read.All, Schedule.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Schedule.Read.All *, Schedule.ReadWrite.All* |

>\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos parâmetros de consulta `$filter` , , , `$orderBy` `$top` `$skipToken` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| MS-APP-ACTS-AS | A ID do usuário em nome do qual o aplicativo está agindo. Obrigatório ao usar o escopo de permissão do aplicativo. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma lista de objetos [timeCard](../resources/timeCard.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação. 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards?$top=2&$filter=state eq 'clockedOut'

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/timecard-list-go-snippets.md)]
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
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.etag": "\"3400c313-0000-0d00-0000-60afe1940000\"",
            "id": "TCK_d1e0f245-9996-4125-b128-d3eb5c4b0164",
            "createdDateTime": "2020-09-21T18:01:29.302Z",
            "lastModifiedDateTime": "2021-05-27T18:14:44.503Z",
            "userId": "66b4f2a4-425d-4dec-8172-7e889950885e",
            "state": "clockedOut",
            "confirmedBy": "none",
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
                "dateTime": "2020-09-21T18:01:29.302Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:14:44.503Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:01:29.302Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:14:44.503Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        },
        {
            "@odata.etag": "\"3400d914-0000-0d00-0000-60afe1ee0000\"",
            "id": "TCK_aa73c610-dd75-4021-bb5c-6b071c7aa835",
            "createdDateTime": "2020-09-21T18:02:48.688Z",
            "lastModifiedDateTime": "2021-05-27T18:16:14.766Z",
            "userId": "3041ccde-7544-4ae0-b44f-3618b08ba1ce",
            "state": "clockedOut",
            "confirmedBy": "none",
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
                "dateTime": "2020-09-21T18:02:48.688Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:16:14.766Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:02:48.688Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:16:14.766Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of timeCard entries in the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
