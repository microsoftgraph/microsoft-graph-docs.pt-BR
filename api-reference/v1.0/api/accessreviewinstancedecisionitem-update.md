---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize as propriedades de um objeto accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6835f91e41032d06c3c96f79fae8be5432dd852d
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697985"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Atualizar accessReviewInstanceDecisionItem
Namespace: microsoft.graph

Atualize as propriedades de [um objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.ReadWrite.All|

Somente um usuário chamador listado como revisor para o [accessReviewInstance](../resources/accessreviewinstance.md) pai pode atualizar **accessReviewInstanceDecisionItem**.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .

A tabela a seguir mostra as propriedades que são aceitas quando você atualiza [o accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Decisão|Cadeia de caracteres|O voto do revisores sobre se a entidade de segurança deve ter acesso ao recurso em revisão. Valores possíveis: `Approve`, `Deny`ou `DontKnow`. Obrigatório.|
|Justificação|Cadeia de Caracteres|O motivo da decisão do revisores. Obrigatório se a **justificationRequiredOnApproval** da propriedade settings do [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) for `true`.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 OK`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstancedecisionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
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



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
