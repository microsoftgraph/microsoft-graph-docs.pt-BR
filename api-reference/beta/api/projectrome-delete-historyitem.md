---
title: Excluir um historyItem
description: Excluir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5a3cac83c220a8fa15a3d5277af319117bd7c927
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264061"
---
# <a name="delete-a-historyitem"></a>Excluir um historyItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excluir um item de histórico existente para uma atividade existente do usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | UserActivity.ReadWrite.CreatedByApp    |
|Delegado (conta pessoal da Microsoft) | UserActivity.ReadWrite.CreatedByApp    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|Autorização | string | {token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Nenhum corpo de solicitação.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `204 No Content` o código de resposta se o item do histórico tiver sido excluído.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_historyItem-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-historyitem.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)"
  ]
}
-->
