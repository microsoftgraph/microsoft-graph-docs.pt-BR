---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 758d78f3f0d844d8913f73a1018206d3e3c14602
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839106"
---
# <a name="delete-grouplifecyclepolicy"></a>Excluir groupLifecyclePolicy

Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---------------|:----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.


## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
