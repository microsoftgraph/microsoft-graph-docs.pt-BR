---
title: Remover appliesTo
description: Remover um directoryObject da adoção de recursos.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d6df64908d05eeb1d5f11faea9218ec4fc5bcfb0
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201537"
---
# <a name="remove-appliesto"></a>Remover appliesTo

Namespace: microsoft.graph

Remova um appliesTo em um [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) para remover [o directoryObject](../resources/directoryobject.md) da rolagem de recursos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{policyId}/appliesTo/{directoryObjectId}/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token}. Obrigatório |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


