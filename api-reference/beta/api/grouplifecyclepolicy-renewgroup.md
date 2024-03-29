---
title: 'groupLifecyclePolicy: renewGroup'
description: Renovar a expiração de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 004743c32f6c6cb7e4dad7c736c45888303e4fe4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202428"
---
# <a name="grouplifecyclepolicy-renewgroup"></a>groupLifecyclePolicy: renewGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Renovar a expiração de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.

> **Nota:** Ao chamar o ponto de extremidade v1.0, use o [método renovar grupo](/graph/api/group-renew?view=graph-rest-1.0&preserve-view=true) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)    |
| :------------------------------------- | :--------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Group.ReadWrite.All ou Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte                                  |
| Aplicativo                            | Group.ReadWrite.All ou Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo | Descrição                   |
| :-------- | :--- | :---------------------------- |
| groupId   | Guid | A ID do grupo a ser renovado. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->

```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/grouplifecyclepolicy-renewgroup-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/grouplifecyclepolicy-renewgroup-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/grouplifecyclepolicy-renewgroup-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/grouplifecyclepolicy-renewgroup-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
