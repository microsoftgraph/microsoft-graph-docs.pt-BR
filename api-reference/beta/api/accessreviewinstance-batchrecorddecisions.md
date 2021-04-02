---
title: 'accessReviewInstance: batchRecordDecisions'
description: Revisores emable para revisar todos os accessReviewInstanceDecisionItems em lotes.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a8bd6778d54100340b0c846230fd8b91b696f1fb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507454"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a>accessReviewInstance: batchRecordDecisions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permitir que os revisores revisem todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em lotes usando `principalId` , ou nenhum `resourceId` deles.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|AccessReviews.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|AccessReviews.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
| decision  | Cadeia de caracteres | Decisão de acesso para a entidade que está sendo revisada. Os valores possíveis são: `Approve`, `Deny`, `NotReviewed`, `DontKnow`. Obrigatório.  |
|  justification | Cadeia de caracteres | Contexto da revisão fornecida aos administradores. Obrigatório se **justificationRequiredOnApproval** `True` estiver no **accessReviewScheduleDefinition**.  |
|principalId|Cadeia de caracteres|Se fornecido, todos os **accessReviewInstanceDecisionItems** com **principalId** correspondente serão revisados neste lote. Se não for fornecido, todos os **principaisIds** serão revisados.|
|resourceId|Cadeia de caracteres|Se fornecido, todos os **accessReviewInstanceDecisionItems** com **resourceId** correspondentes serão revisados neste lote. Se não for fornecido, todos **os resourceIds** serão revisados.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json
Content-length: 113

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
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
