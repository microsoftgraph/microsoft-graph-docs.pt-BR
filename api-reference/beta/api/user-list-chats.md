---
title: Listar chats
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3e8ea297fe707c1076543f925610e30686627a7f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270165"
---
# <a name="list-chats"></a>Listar chats

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de objetos chat.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Chat. Read, chat. ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> [!NOTE]
> O objeto de resposta mostrado aqui pode ser reduzido para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "topic": "topic-value",
      "createdDateTime": "datetime-value",
      "lastUpdatedDateTime": "datetime-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK

# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chats-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chats-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chats-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
