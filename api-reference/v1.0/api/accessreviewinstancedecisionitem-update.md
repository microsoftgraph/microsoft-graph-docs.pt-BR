---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize as propriedades de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 54b66ade8eb217ce740d3d721fc7433c9d86f505
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030993"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Atualizar accessReviewInstanceDecisionItem
Namespace: microsoft.graph

Atualize as propriedades de [um objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.ReadWrite.All|

Somente um usuário de chamada listado como revisor do [accessReviewInstance](../resources/accessreviewinstance.md) pai pode atualizar **o accessReviewInstanceDecisionItem**.

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
No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)

A tabela a seguir mostra as propriedades que são aceitas quando você atualiza [o accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|decision|String|O voto do revistor sobre se a entidade deve ter acesso ao recurso em revisão. Valores possíveis: `Approve` `Deny` , ou `DontKnow` . Obrigatório.|
|justification|String|O motivo da decisão do revistor. Obrigatório se a **justificationRequiredOnApproval** da propriedade settings do [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) for `true` .|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 OK`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstancedecisionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555
Content-Type: application/json
Content-length: 691

{
  "decision": "Approve",
  "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
}
```


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
