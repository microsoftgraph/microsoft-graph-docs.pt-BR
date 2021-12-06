---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize um objeto accessReviewInstanceDecisionItem existente de que chamar o usuário é o revisor.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c83ebbe6b79f987e8c7d523114dd31e570f155df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987716"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Atualizar accessReviewInstanceDecisionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar decisões de acesso, conhecidas como [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), para as quais o usuário é o revisor.

>[!NOTE]
>Todas as atualizações feitas em **um accessReviewInstanceDecisionItem** só podem ser feitas chamando usuários listados como revisores do [accessReviewInstance pai.](../resources/accessreviewinstance.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é necessária para chamar essa API. Não há suporte para permissões delegadas para contas pessoais da Microsoft. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Descrição |
|:-------------|:------------|
|Autorização|{token} de portador. Obrigatório.|
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
A tabela a seguir mostra as propriedades aceitas para atualizar um `accessReviewInstanceDecisionItem` .

| Propriedade     | Tipo       | Descrição |
|:-------------|:------------|:------------|
| decision  | Cadeia de caracteres | Decisão de acesso para a entidade que está sendo revisada. Os valores possíveis são: `Approve` `Deny` `NotReviewed` `DontKnow` . Obrigatório.  |
|  justification | String | Contexto da revisão fornecida aos administradores. Obrigatório se justificationRequiredOnApproval for True no accessReviewScheduleDefinition.  |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `204, NoContent` código de resposta e nenhum corpo de resposta.

### <a name="request"></a>Solicitação
## <a name="examples"></a>Exemplos

Este é um exemplo de aprovação do acesso a um usuário representado por `accessReviewInstanceDecisionItem` um .



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/12348410-67f3-4d4c-b946-6989e050be19
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
