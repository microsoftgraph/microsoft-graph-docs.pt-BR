---
title: 'accessReviewInstance: batchRecordDecisions'
description: Permite que os revisores revisem todos os accessReviewInstanceDecisionItems em lotes.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ea22d510bb70ab8d7047f952f7b4c0e265d57197
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031011"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a>accessReviewInstance: batchRecordDecisions
Namespace: microsoft.graph

Permite que os revisores revisem todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em lotes usando **principalId,** **resourceId** ou nenhum deles.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|AccessReview.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de [um accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).

A tabela a seguir lista as propriedades que você pode usar para revisar [objetos accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|decision|String|Decisão de acesso para a entidade que está sendo revisada. Os valores possíveis são: `Approve`, `Deny`, `NotReviewed`, `DontKnow`. Obrigatório.|
|justification|String|Contexto da revisão fornecida aos administradores. Obrigatório se **justificationRequiredOnApproval** da propriedade settings do **accessReviewScheduleDefinition** for `true` .|
|principalId|String|Se fornecido, todos os **accessReviewInstanceDecisionItems** com valores **principalId** correspondentes serão revisados neste lote. Se não for fornecido, **todos os accessReviewInstanceDecisionItems** serão revisados.|
|resourceId|Cadeia de caracteres|Se fornecido, todos os **accessReviewInstanceDecisionItems** com **resourceId** correspondentes serão revisados neste lote. Se não for fornecido, **todos os accessReviewInstanceDecisionItems** serão revisados.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-6778-8868-9999c7f4cc06/batchRecordDecisions
Content-type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
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
