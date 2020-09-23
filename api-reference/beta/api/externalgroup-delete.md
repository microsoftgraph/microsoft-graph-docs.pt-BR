---
title: Excluir o external
description: Exclui um objeto de um.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 43fb3f0cb0740fe3c7fef23bb244681967cbb13d
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223048"
---
# <a name="delete-externalgroup"></a>Excluir o external

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excluir um [objeto](../resources/externalgroup.md) de um.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (de privilégios máximos a mínimos) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Incompatível                               |
| Delegado (conta pessoal da Microsoft) | Sem suporte                               |
| Aplicativo                            | ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
