---
title: Listar grupos de roteamento de áudio
description: Recupere uma lista de objetos **audioRoutingGroup** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f801fd883d3179863e9151ddcc835c821c98e047
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262283"
---
# <a name="list-audio-routing-groups"></a>Listar grupos de roteamento de áudio

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de objetos **audioRoutingGroup** .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                               |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                               |
| Aplicativo     | Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a>Resposta

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
    {
      "id": "oneToOne",
      "routingMode": "oneToOne",
      "sources": [
        "632899f8-2ea1-4604-8413-27bd2892079f"
      ],
      "receivers": [
        "550fae72-d251-43ec-868c-373732c2704f",
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
