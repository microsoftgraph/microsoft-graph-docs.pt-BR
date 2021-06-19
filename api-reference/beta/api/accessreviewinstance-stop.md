---
title: Parar accessReviewInstance
description: Pare um accessReviewInstance ativo no momento.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c59b08c3a451d54a03502b28d2f05350f38e126f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030485"
---
# <a name="stop-accessreviewinstance"></a>Parar accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Pare um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento. Depois que a instância de revisão de acesso parar, o status da instância será , os revisadores não poderão mais dar entrada e as decisões de revisão de acesso `Completed` podem ser aplicadas.

Parar uma instância não terá efeito em instâncias futuras. Para impedir que uma revisão de acesso recorrente seja iniciar instâncias futuras, [atualize](accessreviewscheduledefinition-update.md) a definição de agendamento para alterar sua data de término agendada.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
Nenhum.

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
